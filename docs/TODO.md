1. degit
2. [express & fastify](https://docs.nestjs.com/first-steps#platform)
3. 快速生成 `controller`: 
   - `nest g resource [name]`
   - `nest g controller [name]`
   - `nest g service [name]`
   - `nest g module [name]`
4. `Injectable` 与 `Inject` 的使用场景
5. `nestjs` 的生命周期
    Incoming Request
      ↓
    [Middleware (Express)]
      ↓
    [Nest Lifecycle]
    ├─> Guard(s)
    ├─> Pipe(s)
    ├─> Interceptor(s)
    └─> Controller Handler
