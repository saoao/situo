## linux学习笔记

查看ip:hostname -I

查看防火墙状态：systemctl status firewalld.service

关闭/开启 开机启动防火墙：systemctl disable/enable firewalld.service

停止防火墙： systemctl stop firewalld.service

开机默认打开网络：

```shell
cd /etc/sysconfig/network-scripts/ 
vi ifcfg-网卡名

```

把ONBOOT=no 改为ONBOOT=yes

# 

CentOS7修改系统显示语言: 中文为英文

vim /etc/locale.conf

LANG="zh_CN.UTF-8"

LANG="en_US.UTF-8"