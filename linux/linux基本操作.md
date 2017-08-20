## Linux安装 ##

#### linux介绍 ####

	Linux 目录

    bin					可执行文件
	sbin				系统可执行文件
	etc					系统的配置文件
	dev					操作底层设备
	home				家目录普通用户目录
	lib/lib64			库文件，jar包
	root				root用户下的目录
	usr					共享资源
	tmp 				临时目录

##### 网络连接模式
NAT模式
![QQ截图20170728005516.png](.\QQ截图20170728005516.png)
所配置的IP地址应该和虚拟交换机在同一段网络

#### linux网络配置 ####
终端输入setup	进入图形界面配置
![PWEXLE7$BC8NNK${N}~72RQ.png](.\PWEXLE7$BC8NNK${N}~72RQ.png)
配置对应的关网
![O6YH7CN$QDB~UW99`2LG419.png](.\O6YH7CN$QDB~UW99`2LG419.png)
重启网络
service network restart


#### linux常用命令 ####
    cd ..							返回上一级
	ifconfig						查看IP地址
    service network restart			重启网络服务
    
#### linux ####