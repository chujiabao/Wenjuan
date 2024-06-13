# chu 表单问卷系统（Spring Boot的实现）



<table>



| 方案    |   Spring Boot + JSP |
|:------| :----: |
| 方案特性  | 原生JS+HTML技术，支持更多浏览器，如IE6 |





chu 表单问卷系统是一款方便、高效、**稳定**的调研问卷系统，一款基于 JAVA WEB 的开源问卷表单系统。


## 浏览器兼容
### 支持现代浏览器和IE6
| IE / Edge | Firefox | Chrome | Safari | Opera |
| :-----| ----: | :----: | :----: | :----: | 
| IE6+,Edge | 支持 | 支持 | 支持 | 支持 | 


参数说明 

`--server.port=8080` 端口

`--spring.datasource.username=root` 数据库账号

`--spring.datasource.password=123456` 数据库账密码

###### 开始使用 

待应用启动完成后，在浏览器输入localhost:8080 即可访问电子调查问卷系统。

### 下载代码本地开发指南

下面是如何使用Spring Boot方案的快速指南。

1、下载代码后，用IDEA打开。

2、然后在idea里面可以直接启动。

4、浏览器访问 localhost:8080

## 数据库脚本、数据初始化

数据库脚本在resources/sql/目录下的dwsurvey.sql数据库脚本文件



	#database settings
	datasource:
    url: jdbc:mysql://localhost:3306/dwsurvey_21test?useUnicode=true&characterEncoding=utf8
    username: root
    password: 123456

    分别修改```url、username、password```

### 部署前创建并初始化dwsurvey数据库

创建数据库，并初始化数据库。

    数据库名：dwsurvey


### 启动访问



配置完成后，启动服务在浏览器中输入如```localhost:8080```相应的地址看到登录页面，表示已经安装成功。

初始账号：```986694345@qq.com``` 密码：```123456```



## 特色

### 全新体验、流程简单


以一种全新的设计体验，告别繁琐的设计流程，通过简单有趣的方式，轻轻松松完成问卷设计，多种问卷样式模板选择，只为显现更精美的表单问卷.

### 丰富的题型 

丰富的题型支持，通过拖拽即可完成题目选择，并可以随意拖动其位置，还可置入所需图片、企业LOGO、设置答题逻辑，一份优美的问卷就是这么简单。

### 问卷表单静态化

对于问卷表单系统，因为所有的表单字段都是后台数据库来维护，所以对于每一次答卷请求，如果都从后端数据库去取每一题及选项的话，必定会对性能造成不小影响。

所以在发布的表单问卷时会对数据进行的页面静态化，生成一个真实的表单存档。

