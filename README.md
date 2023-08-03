# ARL-set
### 源码安装

仅仅适配了 centos 7 ，且灯塔安装目录为/opt/ARL
如果在其他目录可以创建软连接，且安装了四个服务分别为`arl-web`, `arl-worker`, `arl-worker-github`, `arl-scheduler`

```
vim /etc/sysconfig/selinux，SELINUX=disabled，然后保存退出。
wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-cn.sh
chmod +x setup-arl.sh
./setup-arl.sh
```
(./image/selinux.png)

国内安装将wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-github.sh  换成   wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-cn.sh
