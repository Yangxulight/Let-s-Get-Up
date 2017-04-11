# Let-s-Get-Up#
####Life service assistant based on Raspberry####
##基本功能##
       一款基于树莓派的智能寝室生活助手。
* 具有智能早起提醒服务，基于人脸识别技术的早起打卡的监督机制，改善生活作息。
* 同时记录住户的个人健康状况，并且提供一些简单的建议。
* 外接播放器，可以提供氛围音乐的播放。
* 有基于web的控制端，可以在web端完成所有的功能操作。
##硬件需求##
树莓派 摄像头 触摸屏
##技术路线##
* Web页面端负责数据接受显示以及控制的界面
* Django后台负责处理请求并且维护数据库
* 子程序集负责每个子功能实现，例如说早起提醒，氛围音乐播放，以及人脸识别的监督程序等 
	* 人脸识别 open CV 摄像头驱动，照片获取
	* 个人信息 
		* 数据库设计
		* 信息更新
	* 智能早起
		* 定时服务
	* 树莓派完成本地计算，将数据传送至云服务器
	* 用户通过网页客户端访问服务器获取信息

