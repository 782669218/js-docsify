# 拦截器

拦截器是使用 `@Injectable()` 装饰器注解的类。拦截器应该实现 `NestInterceptor` 接口。

![](https://docs.nestjs.com/assets/Interceptors_1.png)

拦截器具有一系列有用的功能，这些功能受面向切面编程（AOP）技术的启发。它们可以：

- 在函数执行之前/之后绑定**额外的逻辑**
- 转换从函数返回的结果
- **转换**从函数抛出的异常
- 扩展基本函数行为
- 根据所选条件完全重写函数 (例如, 缓存目的)

## 基础

每个拦截器都有 `intercept()` 方法，它接收2个参数。 第一个是 `ExecutionContext` 实例（与守卫完全相同的对象）。 `ExecutionContext` 继承自 `ArgumentsHost` 。  `ArgumentsHost` 是传递给原始处理程序的参数的一个包装 ，它根据应用程序的类型包含不同的参数数组。你可以在[这里](https://docs.nestjs.cn/8/exceptionfilters?id=arguments-host)读更多关于它的内容（在异常过滤器章节中）。

### 111
ssss
### 222
2222

