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



1、在Git Bash下，设置user.name和user.email配置信息：

//git config --global user.name "你的GitHub用户名"
//git config --global user.email "你的GitHub注册邮箱"

2、生成ssh密钥文件：

//ssh-keygen -t rsa -C "你的GitHub注册邮箱"

3、将ssh文件同步在github上


oschina的测试方法 ssh -T git@git.oschina.net；成功收到的回复为“Welcome to Git@OSC,‘Your Name’ ”



github的测试方法 ssh -T git@github.com;成功收到的回复为”Hi ’Your Name‘ ! You’ve successfully authenticated, but GitHub does not provide shell access.“


添加公钥：
 ssh-add ~/.ssh/id_rsa