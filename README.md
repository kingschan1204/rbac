# rbac
权限控制平台：

- freemarker
- spring mvc
- spring `4.3.1.RELEASE`
- spring data jpa `1.10.0.RELEASE`
- hiberante `5.1.0.Final`
- logback

springMvc+spring+spring jpa+hibernate ssh搭建


## 开发规范

### action url 规则

- /pub/.* 公共的不需要登录就可以访问
- /admin/模块名称/.* 后台管理严格的权限控制
- /sys/.* 系统管理`除admin以后其它用户一概不允许`

### 包介绍

- common : 能用封装
- model:数据模型，dto`数据传输`,po `持久化对象`,vo `前端页面对象`
- repositories ：数据访问类
- services :业务逻辑处理器
- controller :spring mvc 控制器
- resources : 配置文件，freemarker 模板

## oracle maven install 

mvn install:install-file -Dfile=C:\ojdbc6.jar -DgroupId=com.oracle -DartifactId=ojdbc6 -Dversion=11.2.0.4.0 -Dpackaging=jar
