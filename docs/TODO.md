1. degit
2. [express & fastify](https://docs.nestjs.com/first-steps#platform)
3. 快速生成 `controller`: 
   - `nest g resource [name]`
   - `nest g controller [name]`
   - `nest g service [name]`
   - `nest g module [name]`
4. `Injectable` 与 `Inject` 的使用场景
5. 自定义 `Providers` 以及 `@Optional`
6. `nestjs` 的生命周期
    Incoming Request
      ↓
    [Middleware (Express)]
      ↓
    [Nest Lifecycle]
    ├─> Guard(s)
    ├─> Pipe(s)
    ├─> Interceptor(s)
    └─> Controller Handler
7. [State sharing](https://docs.nestjs.com/controllers#state-sharing) 
   "对于来自其他编程语言的开发者来说，你可能会惊讶地发现，在 Nest 中，几乎所有内容都是在传入请求之间共享的。这包括数据库连接池、具有全局状态的单例服务等等。重要的是要理解，Node.js 不使用请求/响应多线程无状态模型，该模型中每个请求都由单独的线程处理。因此，在 Nest 中使用单例实例对我们的应用程序来说是完全安全的 。"
   TODO: 这个要结合 `learn-nodejs` 重新梳理下