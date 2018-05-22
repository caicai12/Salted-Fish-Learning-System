## Salted-Fish-Learning-System

### 简介

**本学车系统是关于自学驾驶证的应用，随着我国近年来对自学驾驶的推广可以反映出社会的发展和学车过程的开放程度。但是随着自学驾驶证的推广，学员在自学的过程中也出现了越来越多的问题，例如自学过程中所需的教练车、学车场地、职业教练等等。系统主要以解决自学驾驶证所需面临的问题为目的。**

**本系统主要以预约教练学车为中心，扩展相关业务。通过访问学员、教练等方式收集相关学车资料信息，然后通过资料归纳出整个系统的业务功能，最后完成代码编写。学车系统使用 Http 协议实现数据传输和 C/S 架构，客户端与服务端都采用 Java 语言进行编程，其中包括两个客户端以及一个服务器端，完成的功能有发布订单、预约订单、登录/注册、消息中心、预约完成订单、应用帮助等，最后通过系统测试，完善功能之间的关联以及业务的逻辑。**


### 架构

**服务器代码：** NoobStudyCarWeb，采用Java原生Servlet开发，其中主要分三层，分别是表示层、业务逻辑层、数据层

**学员客户端代码：** LearnCarProject

**教练客户端代码：** LearnCarTrainProject

**其中主要使用的技术：**

1. 多线程创建以及管理
2. 二级缓存+网络请求
3. Java锁机制 （多线程共享一片资源时，使用锁的机制来解决多线程冲突的问题）
4. RxJava+Retrofit 网络请求
5. 图片上传以及存储 （上传个人头像到服务器上，服务器进行保存）
6. 定时任务 （定时从服务器上获取消息显示在界面上，通知用户是否有新的消息）
7. 地址定位（学员端使用Android自带的定位方式进行定位、教练端使用高德地图的定位方式进行定位）
