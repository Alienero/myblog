+++
date = "2015-12-03T13:25:16+08:00"
description = ""
title = "IamServer 第一内测版单机搭建"

+++

# 关于IamServer
IamServer 是一个简单的直播流解决方案，使用了OBS->RTMP->IamServer->HTTP-FLV 架构，具体技术细节将不在本文中讨论，本文仅关注于环境的搭建。

## 准备工作
- [OBS](https://obsproject.com/)
- [IamServer 程序](https://github.com/Alienero/IamServer/releases)

## 开始直播吧！
下载完成了IamServer zip文件后，解压缩其为一个独立的文件夹。例如下面图：
![](/livebuild/images/1.png)
在Mac下你需要`cd`到文件夹的内的`bin`目录下启动`./IamServer` ，在windwos下直接启动文件夹内的`IamServer.exe`程序即可。同样在启动程序的时候你可以加上`-name`参数，它可以配置你的直播房间名，不过需要windwos下的同学注意，仅支持`UTF-8`编码哦。如果一切顺利你将看到如下逼格极高的启动画面：
![](/livebuild/images/2.png)
OK，现在配置OBS
![](/livebuild/images/3.png)
URL为`rtmp://localhost/live`,流密钥为`123`,
接下来添加OBS需要捕获的音视频设备，点击串流即可开始发布直播流
![](/livebuild/images/4.png)

IamServer将会监听你电脑所有网卡设备的9090端口，在浏览器里输入你的IP或者域名就直接可以观看直播了
![](/livebuild/images/5.png)
在观看直播的时候输入用户名，就可以和小伙伴的愉快的聊天和玩耍弹幕了，unicode表情是得到支持的哦。在左上角还可以查看当前直播间的观看人数哦。         
大家玩的开心！😄