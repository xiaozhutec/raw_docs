#### 《深入剖析Tomcat》



###### 链接: https://pan.baidu.com/s/1wzEEDDatdPzhE6Go-I1zqg 提取码: p42w


《深入剖析Tomcat》深入剖析Tomcat 4和Tomcat 5中的每个组件，并揭示其内部工作原理。通过学习《深入剖析Tomcat》，你将可以自行开发Tomcat组件，或者扩展已有的组件。 Tomcat是目前比较流行的Web服务器之一。作为一个开源和小型的轻量级应用服务器，Tomcat 易于使用，便于部署，但Tomcat本身是一个非常复杂的系统，包含了很多功能模块。这些功能模块构成了Tomcat的核心结构。《深入剖析Tomcat》从基本的HTTP请求开始，直至使用JMX技术管理Tomcat中的应用程序，逐一剖析Tomcat的基本功能模块，并配以示例代码，使读者可以逐步实现自己的Web服务器。



![](https://img2020.cnblogs.com/blog/2193560/202101/2193560-20210102215344192-818915466.png)


```
目录

《深入剖析Tomcat》
译者序
前 言
第1章 一个简单的Web服务器1
1.1 HTTP1
1.1.1 HTTP请求1
1.1.2 HTTP响应2
1.2 Socket类3
1.3 应用程序5
1.3.1 HttpServer类5
1.3.2 Request类8
1.3.3 Response类10
1.3.4 运行应用程序12
1.4 小结13
第2章 一个简单的servlet容器14
2.1 javax.servlet.Servlet接口14
2.2 应用程序 116
2.2.1 HttpServer1类17
2.2.2 Request类19
2.2.3 Response类21
2.2.4 StaticResourceProcessor类23
2.2.5 servletProcessor1类24
2.2.6 运行应用程序27
2.3 应用程序227
2.4 小结30
第3章 连接器31
3.1 StringManager类31
3.2 应用程序33
3.2.1 启动应用程序35
3.2.2 HttpConnector类36
3.2.3 创建HttpRequest对象38
3.2.4 创建HttpResponse对象49
3.2.5 静态资源处理器和servlet处理器50
3.2.6 运行应用程序50
3.3 小结52
第4章 Tomcat的默认连接器53
4.1 HTTP 1.1的新特性54
4.1.1 持久连接54
4.1.2 块编码54
4.1.3 状态码100的使用55
4.2 Connector接口55
4.3 HttpConnector类56
4.3.1 创建服务器套接字56
4.3.2 维护HttpProcessor实例56
4.3.3 提供HTTP请求服务57
4.4 HttpProcessor类58
4.5 Request对象61
4.6 Response对象62
4.7 处理请求62
4.7.1 解析连接65
4.7.2 解析请求65
4.7.3 解析请求头65
4.8 简单的Container应用程序66
4.9 小结70
第5章 servlet容器71
5.1 Container接口71
5.2 管道任务73
5.2.1 Pipeline接口76
5.2.2 Valve接口76
5.2.3 ValveContext接口76
5.2.4 Contained接口77
5.3 Wrapper接口77
5.4 Context接口78
5.5 Wrapper应用程序78
5.5.1 ex05.pyrmont.core.SimpleLoader类78
5.5.2 ex05.pyrmont.core.SimplePipeline类79
5.5.3 ex05.pyrmont.core.SimpleWrapper类79
5.5.4 ex05.pyrmont.core.SimpleWrapperValve类80
5.5.5 ex05.pyrmont.valves.ClientIPLoggerValve类81
5.5.6 ex05.pyrmont.valves.HeaderLoggerValve类81
5.5.7 ex05.pyrmont.startup.Bootstrap182
5.5.8 运行应用程序84
5.6 Context应用程序84
5.6.1 ex05.pyrmont.core.SimpleContextValve类87
5.6.2 ex05.pyrmont.core.SimpleContextMapper类87
5.6.3 ex05.pyrmont.core.SimpleContext类89
5.6.4 ex05.pyrmont.startup.Bootstrap289
5.6.5 运行应用程序91
5.7 小结92
第6章 生命周期93
6.1 Lifecycle接口93
6.2 LifecycleEvent类94
6.3 LifecycleListener接口94
6.4 LifecycleSupport类95
6.5 应用程序97
6.5.1 ex06.pyrmont.core.SimpleContext类97
6.5.2 ex06.pyrmont.core.SimpleContextLifecycleListener类100
6.5.3 ex06.pyrmont.core.SimpleLoader类101
6.5.4 ex06.pyrmont.core.SimplePipeline类101
6.5.5 ex06.pyrmont.core.SimpleWrapper类101
6.5.6 运行应用程序103
6.6 小结104
第7章 日志记录器105
7.1 Logger接口105
7.2 Tomcat的日志记录器106
7.2.1 LoggerBase类106
7.2.2 SystemOutLogger类107
7.2.3 SystemErrLogger类107
7.2.4 FileLogger类108
7.3 应用程序111
7.4 小结112
第8章 载入器113
8.1 Java的类载入器113
8.2 Loader接口114
8.3 Reloader接口116
8.4 WebappLoader类116
8.4.1 创建类载入器117
8.4.2 设置仓库118
8.4.3 设置类路径118
8.4.4 设置访问权限118
8.4.5 开启新线程执行类的重新载入118
8.5 WebappClassLoader类120
8.5.1 类缓存120
8.5.2 载入类121
8.5.3 应用程序121
8.6 运行应用程序124
8.7 小结124
第9章 Session管理125
9.1 Session对象126
9.1.1 Session接口126
9.1.2 StandardSession类127
9.1.3 StandardSessionFacade类129
9.2 Manager130
9.2.1 Manager接口130
9.2.2 ManagerBase类131
9.2.3 StandardManager类132
9.2.4 PersistentManagerBase类133
9.2.5 PersistentManager类135
9.2.6 DistributedManager类135
9.3 存储器136
9.3.1 StoreBase类137
9.3.2 FileStore类138
9.3.3 JDBCStore类139
9.4 应用程序139
9.4.1 Bootstrap类139
9.4.2 SimpleWrapperValve类140
9.4.3 运行应用程序141
9.5 小结142
第10章 安全性143
10.1 领域143
10.2 GenericPrincipal类144
10.3 LoginConfig类145
10.4 Authenticator接口145
10.5 安装验证器阀146
10.6 应用程序147
10.6.1 ex10.pyrmont.core.SimpleContextConfig类147
10.6.2 ex10.pyrmont.realm.SimpleRealm类149
10.6.3 ex10.pyrmont.realm.SimpleUserDatabaseRealm152
10.6.4 ex10.pyrmont.startup.Bootstrap1类154
10.6.5 ex10.pyrmont.startup.Bootstrap2类156
10.6.6 运行应用程序158
10.7 小结158
第11章 StandardWrapper159
11.1 方法调用序列159
11.2 SingleThreadModel160
11.3 StandardWrapper161
11.3.1 分配servlet实例162
11.3.2 载入servlet类164
11.3.3 ServletConfig对象167
11.3.4 servlet容器的父子关系169
11.4 StandardWrapperFacade类170
11.5 StandardWrapperValve类171
11.6 FilterDef类172
11.7 ApplicationFilterConfig类174
11.8 ApplicationFilterChain类175
11.9 应用程序175
11.10 小结177
第12章 StandardContext类178
12.1 StandardContext的配置178
12.1.1 StandardContext类的构造函数179
12.1.2 启动StandardContext实例179
12.1.3 invoke()方法183
12.2 StandardContextMapper类184
12.3 对重载的支持187
12.4 backgroundProcess()方法188
12.5 小结190
第13章 Host和Engine191
13.1 Host接口191
13.2 StandardHost类193
13.3 StandardHostMapper类195
13.4 StandardHostValve类196
13.5 为什么必须要有一个Host容器197
13.6 应用程序1198
13.7 Engine接口199
13.8 StandardEngine类201
13.9 StandardEngineValve类201
13.10 应用程序2202
13.11 小结203
第14章 服务器组件和服务组件204
14.1 服务器组件204
14.2 StandardServer类206
14.2.1 initialize()方法206
14.2.2 start()方法207
14.2.3 stop()方法207
14.2.4 await()方法208
14.3 Service接口209
14.4 StandardService类211
14.4.1 connector和container211
14.4.2 与生命周期有关的方法213
14.5 应用程序215
14.5.1 Bootstrap类215
14.5.2 Stopper类217
14.5.3 运行应用程序218
14.6 小结219
第15章 Digester库220
15.1 Digester库221
15.1.1 Digester类221
15.1.2 Digester库示例1225
15.1.3 Digester库示例2227
15.1.4 Rule类230
15.1.5 Digester库示例3：使用RuleSet232
15.2 ContextConfig类234
15.2.1 defaultConfig(...
```



***

最后，这里为大家准备了几百本的互联网电子书，有需要的过来取吧。[点击获取](https://mp.weixin.qq.com/s/dFqVQ2qJxvQ0YrIlPISJuw)

*本页书籍均来自网络，如有侵权，请联系我立即删除。我的邮箱：yaojianguolq@163.com*




