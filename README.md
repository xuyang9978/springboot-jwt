# springboot-jwt
## 介绍
SpringBoot 集成 JWT

## 测试步骤
> 测试分两步，首先访问登录接口，登录成功后获取token，然后拿着token在访问查询用户信息接口。
- 1.访问登录接口
    使用 PostMan，访问 http://localhost:8080/login?userName=zhangsan&password=123456，登录成功后接口返回 token
- 2.访问用户信息接口
    使用 PostMan，访问 http://localhost:8080/secure/getUserInfo，header 里需要携带 token信息，key 为“token”，
    value 为刚才登录请求获取到的 token
