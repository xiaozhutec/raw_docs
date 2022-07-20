#### 《轻量级JavaEE企业应用实战》



###### 链接: https://pan.baidu.com/s/1bNYeZHn2OuK1vOsVc6vVWQ 提取码: rtzw





本书介绍了Java EE开发非常流行的三个开源框架：Spring MVC、Spring和MyBatis，其中Spring MVC、Spring用的是5.1版本，MyBatis用的是3.5版本。本书重点介绍了如何整合Spring MVC + Spring + MyBatis进行开发，内容主要包括三部分。部分介绍Java EE开发的基础知识，以及如何搭建开发环境。第二部分详细讲解MyBatis、Spring和Spring MVC三个框架的用法，并从Eclipse IDE的使用上手，一步步带领读者深入三个框架的核心。这部分是本书的核心内容，因此也是重点部分。这部分并不是简单地讲授三个框架的基本用法，而是真正剖析它们在实际开发场景中面临的挑战及佳实践，并对其诸多关键技术实现提供了源代码解读，这样既能加深读者对框架本质的理解，也能直接提升读者的Java功底。第三部分示范开发了一个包含7个表，表之间具有复杂的关联映射、继承映射等关系，且业务也相对复杂的工作流案例，帮助读者理论联系实际，将三个框架真正运用到实际开发中。该案例采用目前非常流行、规范的Java EE架构，整个应用分为领域对象层、Mapper（DAO）。层、业务逻辑层、MVC层和视图层，各层之间分层清晰，层与层之间以松耦合的方式组织在一起。该案例既提供了与IDE无关的、基于Ant管理的项目源代码，也提供了基于Eclipse IDE的项目源代码，大限度地满足读者的需求。本书配有读者答疑交流群，读者可通过扫描本书封面勒口上的二维码，按照指引加入，本书作者将通过交流群提供线上不定期答疑服务。




![](https://img2020.cnblogs.com/blog/2193560/202101/2193560-20210102211249816-370992208.png)



```
第1章 Java EE应用和开发环境 1
1．1 Java EE应用概述 2
1．1．1 Java EE应用的分层模型 2
1．1．2 Java EE应用的组件 3
1．1．3 Java EE应用的结构和优势 4
1．1．4 常用的Java EE服务器 4
1．2 轻量级Java EE应用相关技术 5
1．2．1 JSP、Servlet 4．x和JavaBean及替代技术 5
1．2．2 Spring MVC及替代技术 6
1．2．3 MyBatis及替代技术 6
1．2．4 Spring及替代技术 7
1．3 Tomcat的下载和安装 8
1．3．1 安装Tomcat服务器 8
1．3．2 配置Tomcat的服务端口 9
1．3．3 进入控制台 10
1．3．4 部署Web应用 12
1．3．5 配置Tomcat的数据源 13
1．4 Eclipse的安装和使用 15
1．4．1 Eclipse的下载和安装 15
1．4．2 在线安装Eclipse插件 15
1．4．3 从本地压缩包安装插件 17
1．4．4 手动安装Eclipse插件 18
1．4．5 使用Eclipse开发Java Web应用 18
1．4．6 导入Eclipse项目 21
1．4．7 导入非Eclipse项目 22
1．5 Ant的安装和使用 23
1．5．1 Ant的下载和安装 24
1．5．2 使用Ant工具 25
1．5．3 定义生成文件 26
1．5．4 Ant的任务（task） 30
1．6 Maven的安装和使用 32
1．6．1 下载和安装Maven 33
1．6．2 设置Maven 34
1．6．3 创建、构建简单的项目 35
1．6．4 Maven的核心概念 39
1．6．5 依赖管理 44
1．6．6 POM文件的元素 46
1．7 使用Git进行软件配置管理（SCM） 47
1．7．1 下载和安装Git、TortoiseGit 47
1．7．2 创建本地资源库 49
1．7．3 添加文件和文件夹 51
1．7．4 提交修改 52
1．7．5 查看文件或文件夹的版本变更 53
1．7．6 删除文件或文件夹 54
1．7．7 从以前版本重新开始 55
1．7．8 克隆项目 56
1．7．9 创建分支 56
1．7．10 沿着分支开发 57
1．7．11 合并分支 58
1．7．12 使用Eclipse作为Git客户端 59
1．7．13 配置远程中央资源库 61
1．7．14 推送项目 64
1．7．15 获取项目和拉取项目 64
1．8 本章小结 66

第2章 MyBatis的基础用法 67
2．1 MyBatis是ORM框架吗 68
2．1．1 何谓ORM 68
2．1．2 ORM的映射方式 69
2．1．3 MyBatis的映射方式 70
2．2 MyBatis入门 71
2．2．1 MyBatis的下载和安装 72
2．2．2 MyBatis的数据库操作 72
2．2．3 使用MyBatis执行CRUD 78
2．2．4 利用Mapper对象 80
2．2．5 在Eclipse中使用MyBatis 84
2．3 MyBatis核心API及作用域 90
2．3．1 SqlSessionFactoryBuilder的作用域 90
2．3．2 SqlSessionFactory的作用域 91
2．3．3 SqlSession及其作用域 92
2．3．4 Mapper组件的作用域 94
2．4 MyBatis配置详解 94
2．4．1 属性配置 95
2．4．2 设置配置 98
2．4．3 为类型配置别名 101
2．4．4 对象工厂 103
2．4．5 加载Mapper 105
2．5 类型处理器 106
2．5．1 内置的类型处理器 106
2．5．2 自定义类型处理器 107
2．5．3 枚举的类型处理器 111
2．5．4 存储枚举值的序号 112
2．5．5 同时存储枚举值的名称和序号 113
2．6 数据库环境配置 116
2．6．1 环境配置与默认环境配置 116
2．6．2 事务管理器 117
2．6．3 数据源配置 121
2．6．4 配置第三方C3P0数据源 122
2．7 支持不同类型的数据库 124
2．8 Mapper基础 127
2．8．1 select的用法 128
2．8．2 insert的用法 130
2．8．3 使用useGeneratedKeys返回 自增长的主键值 131
2．8．4 使用selectKey生成主键值 132
2．8．5 update和delete元素的用法 134
2．8．6 使用sql元素定义可复用的SQL片段 134
2．8．7 参数处理 136
2．8．8 参数的额外声明 142
2．8．9 字符串替换 142
2．9 MyBatis代码生成器 144
2．9．1 提供配置文件 145
2．9．2 运行MBG 146
2．10 本章小结 149

第3章 深入使用MyBatis 151
3．1 结果集映射 152
3．1．1 简单resultMap映射 152
3．1．2 构造器映射 154
3．1．3 自动映射 157
3．2 调用存储过程 159
3．2．1 调用返回结果集的存储过程 159
3．2．2 调用带out模式参数的存储过程 160
3．2．3 调用传出参数为游标引用的存储过程 162
3．3 关联映射 165
3．3．1 基于嵌套select的一对一映射 165
3．3．2 基于嵌套select映射策略的性能缺陷 171
3．3．3加载的原理 175
3．3．4 基于多表连接查询的一对一映射 176
3．3．5 基于多结果集的一对一映射 182
3．3．6 基于嵌套select的一对多映射 184
3．3．7 基于多表连接查询的一对多映射 191
3．3．8 基于多结果集的一对多映射 192
3．3．9 多对多映射的三种策略 194
3．4 基于辨别者列的继承映射 201
3．4．1 继承映射的简单示例 201
3．4．2 继承映射的复杂示例 205
3．5 动态SQL 210
3．5．1 if元素的用法 210
3．5．2 在update更新列中使用if 216
3．5．3 在insert动态插入列中使用if 219
3．5．4 choose、when、otherwise元素的 用法 222
3．5．5 where与trim的用法 225
3．5．6 set与trim的用法 228
3．5．7 使用trim实现动态插入 230
3．5．8 foreach元素的基本用法 232
3．5．9 foreach实现批量插入 234
3．5．10 foreach实现批量更新 236
3．5．11 bind元素的用法 239
3．6 缓存 240
3．6．1 一级缓存 240
3．6．2 一级缓存的脏数据与避免方法 243
3．6．3 二级缓存 246
3．6．4 二级缓存的脏数据与避免方法 248
3．6．5 整合Ehcache实现二级缓存 252
3．7 用插件扩展MyBatis 254
3．7．1 拦截器接口及作用原理 254
3．7．2 可拦截的目标 256
3．7．3 为MyBatis开发分页插件 260
3．8 本章小结 266

第4章 Spring的基础用法 267
4．1 Spring简介和Spring 5的变化 268
4．1．1 Spring简介 268
4．1．2 Spring 5．x的变化 269
4．2 Spring入门 269
4．2．1 Spring的下载和安装 270
4．2．2 使用Spring管理Bean 270
4．2．3 在Eclipse中使用Spring 274
4．3 Spring的核心机制：依赖注入 276
4．3．1 理解依赖注入 277
4．3．2 设值注入 278
4．3．3 构造注入 282
4．3．4 两种注入方式的对比 284
4．4 使用Spring容器 284
4．4．1 Spring容器 284
4．4．2 使用ApplicationContext 286
4．4．3 ApplicationContext的化支持 287
4．4．4 ApplicationContext的事件机制 289
4．4．5 让Bean获取Spring容器 292
4．5 Spring容器中的Bean 294
4．5．1 Bean的基本定义和Bean别名 294
4．5．2 容器中Bean的作用域 295
4．5．3 配置依赖 299
4．5．4 设置普通属性值 300
4．5．5 配置合作者Bean 302
4．5．6 使用自动装配注入合作者Bean 302
4．5．7 注入嵌套Bean 305
4．5．8 注入集合值 306
4．5．9 组合属性 311
4．5．10 Spring的Bean和JavaBean 312
4．6 Spring的Java配置管理 313
4．7 创建Bean的三种方式 316
4．7．1 使用构造器创建Bean 316
4．7．2 使用静态工厂方法创建Bean 317
4．7．3 使用实例工厂方法创建Bean 319
4．8 深入理解容器中的Bean 321
4．8．1 抽象Bean与子Bean 322
4．8．2 Bean继承与Java继承的区别 323
4．8．3 容器中的工厂Bean 323
4．8．4 获得Bean本身的id 326
4．8．5 强制初始化Bean 327
4．9 容器中Bean的生命周期 327
4．9．1 依赖关系注入之后的行为 328
4．9．2 Bean销毁之前的行为 330
4．9．3 协调作用域不同步的Bean 332
4．10依赖关系配置 336
4．10．1 获取其他Bean的属性值 336
4．10．2 获取Field值 339
4．10．3 获取方法的返回值 341
4．11 基于XML Schema的简化配置方式 344
4．11．1 使用p：命名空间简化配置 344
4．11．2 使用c：命名空间简化配置 345
4．11．3 使用util：命名空间简化配置 347
4．12 Spring表达式语言 349
4．12．1 使用Expression接口进行表达式求值 350
4．12．2 Bean定义中的表达式语言支持 352
4．12．3 SpEL语法详述 353
4．13 本章小结 358

第5章 深入使用Spring 359
5．1 两种后处理器 360
5．1．1 Bean后处理器 360
5．1．2 Bean后处理器的用处 364
5．1．3 容器后处理器 364
5．1．4 属性占位符配置器 366
5．1．5 重写占位符配置器 367
5．2 “零配置”支持 368
5．2．1 搜索Bean类 368
5．2．2 指定Bean的作用域 371
5．2．3 使用@Resource、@Value配置依赖 372
5．2．4 使用@PostConstruct和@PreDestroy定制生命周期行为 373
5．2．5 @DependsOn和@Lazy 374
5．2．6 自动装配和装配 374
5．2．7 Spring 5新增的注解 379
5．3 资源访问 380
5．3．1 Resource实现类 381
5．3．2 ResourceLoader接口和 ResourceLoaderAware接口 385
5．3．3 使用Resource作为属性 388
5．3．4 在ApplicationContext中使用资源 389
5．4 Spring的AOP 392
5．4．1 为什么需要AOP 393
5．4．2 使用AspectJ实现AOP 394
5．4．3 AOP的基本概念 401
5．4．4 Spring的AOP支持 402
5．4．5 基于注解的“零配置”方式 403
5．4．6 基于XML配置文件的管理方式 418
5．5 Spring的缓存机制 424
5．5．1 启用Spring缓存 425
5．5．2 使用@Cacheable执行缓存 427
5．5．3 使用@CacheEvict清除缓存数据 431
5．6 Spring的事务 433
5．6．1 Spring支持的事务策略 433
5．6．2 使用XML Schema配置事务策略 436
5．6．3 使用@Transactional 442
5．7 Spring整合MyBatis 443
5．7．1 整合MyBatis的关键点及快速入门 443
5．7．2 配置SqlSessionFactory 448
5．7．3 通过工厂Bean配置Mapper组件 449
5．7．4 通过扫描自动配置Mapper组件 450
5．7．5 基于SqlSession实现DAO组件 452
5．7．6 继承SqlSessionDaoSupport实现DAO组件 455
5．7．7 事务管理 457
5．8 本章小结 458

第6章 Spring MVC的基础用法 459
6．1 MVC概述 460
6．1．1 MVC模式及其优势 460
6．1．2 Spring MVC与Struts 2的区别 461
6．2 Spring MVC入门 463
6．2．1 在Web应用中启动Spring容器 463
6．2．2 配置核心控制器 466
6．2．3 开发控制器 468
6．2．4 提供视图资源 470
6．2．5 使用Eclipse开发Spring MVC应用 471
6．3 Spring MVC的流程 472
6．3．1 Spring MVC应用的开发步骤 472
6．3．2 Spring MVC的运行流程 474
6．3．3 DispatcherServlet详解 475
6．3．4 mvc：annotation-driven详解 480
6．4 静态资源处理 481
6．4．1 静态资源映射 481
6．4．2 配置默认Servlet 483
6．5 视图解析器 485
6．5．1 UrlBasedViewResolver的功能与用法 486
6．5．2 InternalResourceViewResolver的功能与用法 491
6．5．3 XmlViewResolver及视图解析器的链式处理 492
6．5．4 ResourceBundleViewResolver的功能与用法 496
6．5．5 BeanNameViewResolver的功能与用法 497
6．5．6 重定向视图 499
6．5．7 将数据传给重定向目标 500
6．5．8 ContentNegotiatingViewResolver的功能与用法 503
6．6 请求映射与参数处理 510
6．6．1 HandlerMapping与处理映射 510
6．6．2 SimpleUrlHandlerMapping的功能与用法 511
6．6．3 @RequestMapping注解及其变体 512
6．6．4 处理方法允许的返回值类型 515
6．6．5 @RequestParam注解与MultiValueMap 516
6．6．6 使用@PathVariable获取路径变量的值 520
6．6．7 使用@PathVariable处理正则 表达式 523
6．6．8 路径模式 524
6．6．9 使用@MatrixVariable处理Matrix变量 526
6．6．10 使用@RequestHeader获取请求头的值 529
6．6．11 异步处理 530
6．6．12 使用DeferredResult支持异步处理 534
6．6．13 使用@ModelAttribute修饰方法本身 536
6．6．14 使用@ModelAttribute修饰方法参数 539
6．7 将数据传给视图页面 541
6．7．1 Model、ModelMap和RedirectAttributes 541
6．7．2 使用@SessionAttributes添加session属性 542
6．8 RESTful服务支持 544
6．8．1 RESTful简介 544
6．8．2 @RequestBody与@ResponseBody注解 546
6．8．3 HttpMessageConverter与消息转换 550
6．8．4 转换XML数据 553
6．8．5 使用@RestController修饰RESTful控制器 557
6．8．6 @CrossOrigin注解与跨域请求 557
6．9 访问Servlet API相关数据 561
6．9．1 处理方法可接受的形参类型 561
6．9．2 使用@RequestAttribute获取请求属性 562
6．9．3 使用@SessionAttribute获取session属性 563
6．9．4 直接访问Servlet API 566
6．9．5 使用WebRequest和NativeWebRequest伪访问 567
6．9．6 使用@CookieValue获取cookie值 569
6．9．7 在处理方法中使用IO流 571
6．10 本章小结 573

第7章 深入使用Spring MVC 574
7．1化 575
7．1．1化到底怎么做 575
7．1．2 根据浏览器请求头确定Locale 577
7．1．3 根据session确定Locale 582
7．1．4 根据cookie值确定Locale 586
7．2 异常处理 587
7．2．1 Spring MVC异常处理 587
7．2．2 传统的异常处理机制 590
7．2．3 使用@ResponseStatus修饰异常类 594
7．2．4 使用@ExceptionHandler修饰异常 处理方法 596
7．2．5 使用@ControllerAdvice定义异常Aspect 599
7．2．6 使用@RestControllerAdvice定义异常Aspect 600
7．3 标签库 602
7．3．1 form标签与普通表单域标签 602
7．3．2 radiobutton和radiobuttons标签 605
7．3．3 checkbox和checkboxes标签 607
7．3．4 select和option、options标签 610
7．3．5 htmlEscape和escapeBody标签 612
7．3．6 url和param标签 613
7．4 类型转换与绑定 615
7．4．1 BeanWrapper简介 616
7．4．2 PropertyEditor与内置实现类 618
7．4．3 自定义PropertyEditor 619
7．4．4 使用WebBindingInitializer注册全局PropertyEditor 621
7．4．5 使用ConversionService执行转换 623
7．4．6 处理转换 626
7．5 格式化 629
7．5．1 使用格式化器 630
7．5．2 使用FormatterRegistrar注册 格式化器 633
7．6 数据校验 634
7．6．1 使用Validation执行校验 634
7．6．2 基于JSR 303执行校验 638
7．7 文件上传与下载 641
7．7．1 使用MultipartFile处理文件上传 641
7．7．2 基于Commons FileUpload组件 上传文件 646
7．7．3 使用@RequestPart注解 647
7．7．4 文件下载 650
7．7．5 下载前的授权控制 652
7．8 拦截器 653
7．9 SSM整合开发 656
7．9．1 搭建项目 657
7．9．2 开发Mapper组件 659
7．9．3 开发Service组件 660
7．9．4 控制器与视图 661
7．10 本章小结 666

第8章 简单工作流 667
8．1 项目背景及结构 668
8．1．1 应用背景 668
8．1．2功能介绍 668
8．1．3 相关技术介绍 669
8．1．4结构 670
8．1．5的功能模块 670
8．2 领域对象层 671
8．2．1 设计领域对象 671
8．2．2 创建领域对象类 672
8．3 实现Mapper（DAO）层 677
8．3．1 Mapper组件的定义 677
8．3．2 实现Mapper组件 681
8．3．3 部署Mapper层 685
8．4 实现Service层 686
8．4．1 业务逻辑组件的设计 686
8．4．2 实现业务逻辑组件 687
8．4．3 事务管理 692
8．4．4 部署业务逻辑组件 693
8．5 实现任务的自动调度 693
8．5．1 使用Quartz 693
8．5．2 在Spring中使用Quartz 698
8．6 实现Web层 700
8．6．1 配置核心控制器和启动Spring容器 700
8．6．2 控制器的处理顺序 701
8．6．3 员工登录 702
8．6．4 进入打卡 705
8．6．5 处理打卡 707
8．6．6 进入申请 708
8．6．7 提交申请 709
8．6．8 使用拦截器完成权限管理 710
8．7 本章小结 712


```



***

最后，这里为大家准备了几百本的互联网电子书，有需要的过来取吧。[点击获取](https://mp.weixin.qq.com/s/dFqVQ2qJxvQ0YrIlPISJuw)

*本页书籍均来自网络，如有侵权，请联系我立即删除。我的邮箱：yaojianguolq@163.com*

