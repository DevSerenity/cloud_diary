
#### 介绍
一款用于个人日常记录，旅游是，生活的个人备忘录系统，系统采用 B/S 架构，使用 BootStrap + Jsp + Servlet + MySQL+ Tomcat 开发，使用 Maven 构建，采用 Junit 单元测试、Log4j 搭建日志、使用 POI 导入导出报表，操作 DB 使用大名鼎鼎的 DBUtil
#### 软件架构
软件架构说明：
    本项目包含用户模块、类型模块、云记模块、数据报表、首页模块这几个核心模块
#### 文件架构
|---src  
    |---main // 主包  
        |---java // 源程序  
            |---com.myDemo.note  
                |---dao // 数据对象   
                |---po // 实体类  
                |---vo // 视图对象  
                |---service // 业务类  
                |---web  // 控制类  
                |___util // 工具类  
        |---resources // 插件资源  
        |___webapp // 网站资源  
    |___test // 单元测试  
|---pom.xml // 配置文件

#### 技术选型

1.  JSP
2.  Servlet
3.  Jquery及插件
4.  Ueditor
5.  log4j
6.  Junit

#### 技术细节
1.  技术细节
2.  增删改查
3.  免登录：Session 和 Cookie
4.  非法访问：过滤器 Filter
5.  文件上传
6.  分页
7.  Ajax：Dom操作
8.  富文本编辑器

#### 开发环境

    IDEA + Maven + MySQL + Jdk1.8 + Tomcat

#### 数据库设计

- user用户表

| 字段名称   | 字段类型    | 字段描述  |
|--------|---------|-------|
| userId | int     | 主键，自增 |
| uname  | varchar | 用户名称  |
| upwd   | varchar | 用户名称  |
| nick   | varchar | 用户昵称  |
| head   | varchar | 用户头像  |
| mood   | varchar | 用户心情  |

- note_type类型表

| 字段名称     | 字段类型    | 字段描述  |
|---------|----------|-------|
| typeId   | int     | 主键，自增 |
| typeName | varchar | 类型名称  |
| userId   | int     | 用户ID  |

- note日记表

| 字段名称    | 字段类型     | 字段描述  |
|---------|----------|-------|
| noteId  | int      | 主键，自增 |
| title   | varchar  | 标题    |
| content | text     | 内容    |
| typeId  | int      | 类型ID  |
| pubTime | datetime | 发布时间  |
| lon     | float    | 经度    |
| lat     | float    | 纬度    |


#### 相关截图

![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/login.png)
![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/user.png)
![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/date.png)
![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/list.png)
![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/out.png)
![输入图片说明](reference/002_%E9%9D%99%E6%80%81%E8%B5%84%E6%BA%90/images/index.png)# CloudDiary


#### 参与贡献

1.  Fork 本仓库
2.  新建 Feat_xxx 分支
3.  提交代码
4.  新建 Pull Request


#### 特技

1.  使用 Readme\_XXX.md 来支持不同的语言，例如 Readme\_en.md, Readme\_zh.md
2.  Gitee 官方博客 [blog.gitee.com](https://blog.gitee.com)
3.  你可以 [https://gitee.com/explore](https://gitee.com/explore) 这个地址来了解 Gitee 上的优秀开源项目
4.  [GVP](https://gitee.com/gvp) 全称是 Gitee 最有价值开源项目，是综合评定出的优秀开源项目
5.  Gitee 官方提供的使用手册 [https://gitee.com/help](https://gitee.com/help)
6.  Gitee 封面人物是一档用来展示 Gitee 会员风采的栏目 [https://gitee.com/gitee-stars/](https://gitee.com/gitee-stars/)
