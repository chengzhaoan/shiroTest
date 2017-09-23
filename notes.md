## 本测试过程基于如下文档  
* [跟我学Shiro](http://www.iteye.com/blogs/subjects/shiro)
### UsernamePasswordToken  
```
      private String username;
      private char[] password;
      private boolean rememberMe = false;                  
      private String host;
      
      username     =   Principal
      Password     =   Credentials
```
### AuthenticationToken
    这个接口只有两个method
```
   get
       Principal
       Credentials
```

testCustomRealm()  
    中使用Realm提供了用户名和密码的验证，取代了helloworld的配置用户名密码的配置文件
    securityManager.realms=$myRealm1  
    这个配置内容提供用户名密码的的验证服务
    其实内容也不多