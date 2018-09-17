# Pi Dashboard
Pi 仪表盘 - 物联网IoT设备炫酷的WebUI监控工具

A WebUI dashboard for IoT devices likes raspberry pi.

Project details: (http://maker.quwj.com/project/10)

Copyright 2017 NXEZ.com.
------------------
#详细说明
Pi Dashboard (Pi 仪表盘) 是一个开源的 IoT 设备监控工具，目前主要针对树莓派平台，也尽可能兼容其他类树莓派硬件产品。你只需要在树莓派上安装好 PHP 服务器环境，即可方便的部署一个 Pi 仪表盘，通过炫酷的 WebUI 来监控树莓派的状态！

目前已加入的监测项目有：

CPU 基本信息、状态和使用率等实时数据
内存、缓存、SWAP分区使用的实时数据
SD卡（磁盘）的占用情况
实时负载数据
实施进程数据
网络接口的实时数据
树莓派IP、运行时间、操作系统、HOST 等基础信息

仪表盘预览
http://shumeipai.nxez.com/wp-content/uploads/2017/08/20170831005933963-0.jpg

安装方法

安装共2步，首先安装 Nginx（或 Apache）和 PHP。然后在 Nginx 目录通过 SFTP 或 GitHub 部署好本项目的程序。
1.安装 Nginx 和 PHP
2.部署 Pi Dashboard
这里介绍两种方法将 Pi Dashboard 部署在 Nginx 上。
2.1. SFTP 上传
在 GitHub 下载本项目源码。通过 FileZilla 等 FTP 软件将解压出来的目录上传到web根目录下。
那么可以通过 http://IP地址/pi-dashboard 访问部署好了的 Pi Dashboard。
如果页面无法显示，可以尝试在树莓派终端给源码添加运行权限，例如你上传之后的路径是 /var/www/html/pi-dashboard，则运行。
cd /var/www/html
sudo chown -R www-data pi-dashboard

2.2. GitHub 部署
如果你了解过 GitHub 的基本操作，通过 GitHub 来下载本项目到 Pi 上会相当方便。

#如果已安装过 git 客户端可以跳过下一行
sudo apt-get install git
cd /var/www/html
sudo git clone https://github.com/spoonysonny/pi-dashboard.git

即可通过 http://IP地址/pi-dashboard 访问部署好了的 Pi Dashboard。

同样如果页面无法显示，可以尝试在树莓派终端给源码添加运行权限，例如你上传之后的路径是 /var/www/html/pi-dashboard，则运行。

cd /var/www/html
sudo chown -R www-data pi-dashboard

========================================
一下是自用克隆源代码，需要的请自助安装。

//克隆可道云
[root@centos-rpi2]# git clone https://github.com/kalcaddle/KODExplorer.git
[root@centos-rpi2]# chmod -Rf 777 ./KODExplorer/*

==================

//克隆DzzOffice开源办公套件

[root@centos-rpi2]# git clone https://github.com/zyx0814/dzzoffice.git

[root@centos-rpi2]# chmod -Rf 777 ./*

==================

//克隆XiunoBBS -轻论坛 

[root@centos-rpi2]# git clone https://gitee.com/xiuno/xiunobbs.git  

[root@centos-rpi2]# chmod -Rf 777 ./xiunobbs/*

==================

//克隆Typecho博客平台

[root@centos-rpi2]# git clone https://github.com/typecho/typecho.git

[root@centos-rpi2]# chmod -Rf 777 ./typecho/*

主题 ：

大前端 https://git.coding.net/Arco-X/DUX-for-Typecho.git

大姐姐 https://git.coding.net/Arco-X/H-Code.git

小清新https://github.com/chakhsu/pinghsu.git


插件：

标签自动生成 https://github.com/DT27/AutoTags.git

Markdown 编辑器 https://github.com/DT27/EditorMD.git


==================

//爱特PHP网站文件管理专家

[root@centos-rpi2]# wget https://aite.me/fileadmin.zip

[root@centos-rpi2]# unzip fileadmin.zip

[root@centos-rpi2]# chmod -Rf 777 ./*


==================

//克隆FluxBB -轻论坛 

[root@centos-rpi2]# git clone https://github.com/fluxbb/fluxbb.git

[root@centos-rpi2]# chmod -Rf 777 ./*


语言包https://github.com/fluxbb/langs


==================

//克隆Pi Dashboard (Pi 仪表盘) IoT 设备监控工具，提供 Web UI 仪表盘面板

[root@centos-rpi2]# git clone https://github.com/joyist2018/pi-dashboard.git  （中文版源）

git clone https://github.com/spoonysonny/pi-dashboard.git （英文版源）


[root@centos-rpi2]# chmod -Rf 777 ./*


==================

//克隆HTML5 Speedtest 网站测速

[root@centos-rpi2]# git clone https://github.com/adolfintel/speedtest.git

[root@centos-rpi2]# chmod -Rf 777 ./*


==================

//克隆 ImgURL轻便图床源码

[root@centos-rpi2]# git clone https://github.com/helloxz/imgurl.git

[root@centos-rpi2]# chmod -Rf 777 ./*





