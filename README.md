**项目使用技术** ：

springboot + mybatisplus+redis+mysql

**项目讲解说明：**

1. 提供前端工程，只需要实现后端接口即可
2. 项目以单体架构入手，先快速开发，不考虑项目优化，降低开发负担
3. 开发完成后，开始优化项目，提升编程思维能力
4. 比如页面静态化，缓存，云存储，日志等
5. docker部署上线
6. 云服务器购买，域名购买，域名备案等

**总结**
jwt + redis

token令牌的登录方式,访问速度快,session共享,安全性

redis做了令牌和用户信息的对应管理, 1.进一步增加了安全性 2.登录用户做了缓存,灵活 控制用户的过期(续期,踢掉线等)

ThreadLocal 使用保存用户信息,请求的线程之内,可以随时获取登录的用户,做了线程隔离

使用完ThreadLocal之后,做了value删除,防止内存泄露

线程安全-update table set value = newValue where id=1 and value=oldValue

旧值的基础上更新新值,防止并发出现的问题

线程池 应用非常广,七个核心参数(对当前的主业务 无影响的操作,放入线程池执行)

登录,记录日志(要求互不影响)

权限系统(SpringSecurity)

统一日志记录,统一缓存处理