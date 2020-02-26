Table of Contents
=================

   * [基于部标jt808的冷链物流车辆调度管理系统](#基于部标jt808的冷链物流车辆调度管理系统)
      * [项目介绍：](#项目介绍)
         * [技术要点：](#技术要点)
   * [在线Demo:](#在线demo)
   * [功能模块图：](#功能模块图)

目录生成插件 [gh-md-toc](https://github.com/ekalinin/github-markdown-toc)



# 基于部标jt808的冷链物流车辆调度管理系统

## 项目介绍：

了解部标JT808协议，完成部分协议功能，设计并实现一个车辆调度管理系统。物流管理员通过网页进行各种信息的管理、订单分配和车辆调度；司机可以通过网页获取路径推荐，接收指令。

主要功能包括车辆信息管理、车载终端信息管理、订单管理、车辆调度、车辆轨迹管理。

个人所用技术：java、netty、springboot、mysql、mybatis、redis、vue、nginx、websocket

### 技术要点：

1.服务端与车载终端交互：利用springboot + netty根据JT808协议实现；

2.服务端与前端交互：利用vue+element-ui+springMVC完成页面开发，其中，与司机的沟通利用websocket实现

3.数据层：利用mybatis+mysql进行DAO层开发，利用redis缓存部分业务数据；

4.项目部署：前后端分离部署，利用nginx反向代理

5.实现算法模块：历史路径压缩模块和最短路径推荐模块。



# 在线Demo:

<http://129.204.127.197:8081/#/>

管理员界面不需要帐号密码

司机界面是013800010002



# 功能模块图：

![功能模块图](https://i.loli.net/2020/02/26/vlqMzp1PNdBxDQ4.png)
