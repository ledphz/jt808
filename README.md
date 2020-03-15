# 基于部标jt808的冷链物流车辆调度管理系统

# 在线Demo:

<http://129.204.127.197:8081/#/



<br>项目时间：2019.09--2020.02（历时6个月）

<br>项目描述：了解交通部标准《JT808协议》，完成部分协议功能，设计并实现一个物流车辆调度管理系统。每辆物流配送车辆装有一个车载终端，主要负责定位。物流管理员通过Web界面管理订单、车辆、车载终端信息，进行订单分配、指令下发、查看历史轨迹。物流司机通过Web界面接收指令、获取最短路径推荐。

<br>主要功能：最短路径推荐、历史轨迹压缩、车辆管理、车载终端管理、订单管理、车辆调度策略。

<br>项目所用技术：Java、Netty、Spring Boot、MySQL、MyBatis、Redis、Vue、Nginx、WebSocket、BaiduMap

<br>技术要点：

1.根据《JT808协议》，使用Netty对服务端与车载终端的消息进行解析；

2.使用Vue + Spring MVC完成前端页面开发与接口交互，部分接口采用Restful设计；

3.使用MyBatis + MySQL进行DAO层开发，部分数据采用Redis存储；

4.算法模块：改进Douglas–Peucker算法并实现历史路径压缩模块；使用Dijkstra算法实现最短路径推荐模块；

5.使用WebSocket实现服务器端与司机端的双向通信，使用BaiduMap实现地图展示；

6.前后端分离开发、部署，使用Nginx代理。





# 功能模块图：

![图挂了打开https://i.loli.net/2020/03/15/hSVxGN52vE4aHPg.png](https://i.loli.net/2020/03/15/hSVxGN52vE4aHPg.png)
