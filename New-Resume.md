 <center>
     <h1>董洋</h1>
     <div>
         <span>
             <img src="assets/phone-solid.svg" width="18px">
           15036616562
         </span>
         ·
         <span>
             <img src="assets/envelope-solid.svg" width="18px">
             yyancy517@gmail.com
         </span>
         ·
         <span>
             <img src="assets/github-brands.svg" width="18px">
             <a href="https://github.com/yyancy">github.com/yyancy</a>
         </span>
         ·
     </div>
 </center>

## <img src="assets/info-circle-solid.svg" width="30px"> 个人信息

- 男，汉族
- 求职意向：Java 开发工程师
- 工作经验：6 年

## <img src="assets/graduation-cap-solid.svg" width="30px"> 教育经历

- 自考本科，郑州大学，计算机科学与技术专业，2018.9~2021.6

## <img src="assets/briefcase-solid.svg" width="30px"> 工作经历

- 上海网达软件股份有限公司，研发部门，JAVA 工程师，2022.10-至今
- 郑州新光源电子科技有限公司，研发部门，JAVA 工程师，2018.9-2022.9

## <img src="assets/tools-solid.svg" width="30px"> 技能清单

- 拥有六年以上的 Java 及 Java Web 开发经验，具有扎实的程序设计基本功，能够独立承担功能模块的开发设计
- 熟练使用 Java 编程语言，了解 Python，Go 等编程语言
- 理解常用的设计模式并能够合理应用 java 新特性，如 Stream API,lambda 表达式,函数式编程等
- 熟练使用 Spring boot,Spring Cloud,Mybatis 等框架技术，有实际项目开发经验
- 熟悉消息中间件技术，如 RabbitMQ 以及分布式缓存技术，例如 redis
- 熟练使用数据库 MySQL 以及数据库开发辅助工具进行操作,并且熟悉使用 SQL 语言
- 熟悉 Docker、Jekins、Linux，有 Linux 服务器项目部署经验，
- 可以在 linux 系统上熟练开发，掌握 java 配置，tomcat 配置，nginx 配置以及 mysql 配置，并部署过系统上线
- 熟练使用 IDEA、Git、Maven 等常用开发工具, 拥有 shell/Python 脚本开发经验
- 熟练应用 Java 集成开发环境(IDE) IDEA,以及 vscode 和 vim 编辑器

## <img src="assets/project-diagram-solid.svg" width="30px"> 项目经历

### <img src="assets/briefcase-solid.svg" width="30px"> 上海网达软件股份有限公司
- **智能视频云网关中实现35114协议**
- **智能视频云网关系统国产化**
- **下载视频流水印功能**
- **多个系统网关平台部署**
- **iot系统功能迁移**
- **智能视频云网关添加租户功能**
- **视联网平台添加自动化部署脚本**

### <img src="assets/briefcase-solid.svg" width="30px"> 郑州新光源电子科技有限公司

- **郑州 12345 便民热线系统知识库模块的设计与开发**

  郑州市 12345 热线系统是用来解决市民问题的政务处理系统，其中知识库模块是用来支持前台坐席查询常用信息，政务公告，内部知识库等内容。

  负责整个模块的开发与设计。在与坐席沟通需求后，设计了提问，审核，回答，再次审核的流程模块，以及各单位知识库，总知识库以及其他相关分类管理功能。在坐席提问相关单位并审核通过后，使用 activeMQ 来通知下级单位用户并发送短信。

  此系统使用 Spring boot 来作为后台框架开发，使用 Mysql 来做数据存储。

  随着系统上线一段时间后，坐席反映知识库响应过于缓慢。经过查询日志之后发现，随着知识库数量的增加，数据库查询成为瓶颈。之后使用 elasticsearch 索引搜索，提升了知识库检索速度。

- **郑州 12345 便民服务热线系统环境搭建与上线部署**

  在私有云上搭建 12345 热线系统运行环境。

  系统架构为 4 台 Mysql 数据库进行双主双备，用 2 台 Mycat 来连接数据库并使用 keepalived 进行高可用。4 台 tomcat 后端服务，2 台 nginx 进行负载均衡以及访问前端，并使用 keepalived 进行高可用。以及 activeMQ 服务器，elasticsearch 服务器。

  使 ssh 连接至 ubuntu 服务器，安装基本依赖包例如 vim，gcc 等。之后按照每台服务器功能安装相应的软件。

  服务器安装部署完成后，迁移数据库并部署程序。测试系统功能。

- **郑州市便民热线二级平台处理系统工单流转处理模块**

  系统为 12345 热线系统的二级平台，其作用是为二级单位提供将工单转办至三级单位处理流程。

  负责整个工单流程模块的开发。其中主要包括接收工单，转办工单，办结工单审核以及重办，退回流程。每步操作都插入一条操作记录，方便回溯工单处理流程。

  使 Spring Boot 来做后台框架开发，Mysql 数据库存储。使用 Spring 的事务集成来处理可能会出现的异常情况，保证数据的一致性。案件转办至下级单位后，使用 activeMQ 通知下级单位工单并发送短信。

- **郑州 12345 便民热线合并市长信箱**

  本系统为对接系统，即将市长信箱集成至热线系统。将市民登记的信箱案件按照热线系统的工单流程处理。

  负责整个项目的开发并根据现有的信箱接口和流程来进行开发。使用政务第三方认证平台来进行用户认证，并保存相关凭证。

  使用 Spring Boot 进行后台开发并以 jar 方式运行。使用 nginx 作为前端服务器。在系统上线一段时间后，根据新要求更改 http 访问为 https 并解决 CORS 问题。

- **濮阳市智慧物业系统开发**

  本系统为濮阳市房管局辅助处理系统。其会接听市民的来电电话登记工单，并将相关工单转办至主系统进行处理。主流程系统会调用相关的回调方法来推送当前工单状态，方便前台查询。当主系统办结后，会调用当前系统的办结回调方法来进行相关后续操作。

  主要负责对接接口以及回调方法的开发。与主系统技术人员沟通相关接口参数以及调用方式。开发完成后进行上线测试。

  使用 Spring Boot 开发，部署在 tomcat 中运行，并使用 tomcat 来作为前端服务器。
