# ARL-set
### 源码安装

仅仅适配了 centos 7 ，且灯塔安装目录为/opt/ARL
安装前必须关闭防火墙和selinux
```
vim /etc/sysconfig/selinux，SELINUX=disabled，然后保存退出。默认：#SELINUX=enforcing
```
下面是/etc/sysconfig/selinux默认文件的配置

```
# This file controls the state of SELinux on the system.
# SELINUX= can take one of these three values:
#     enforcing - SELinux security policy is enforced.
#     permissive - SELinux prints warnings instead of enforcing.
#     disabled - No SELinux policy is loaded.
SELINUX=enforcing
# SELINUXTYPE= can take one of three values:
#     targeted - Targeted processes are protected,
#     minimum - Modification of targeted policy. Only selected processes are protected.
#     mls - Multi Level Security protection.
SELINUXTYPE=targeted
```

如果在其他目录可以创建软连接，且安装了四个服务分别为`arl-web`, `arl-worker`, `arl-worker-github`, `arl-scheduler`

```
wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-cn.sh
chmod +x setup-arl.sh
./setup-arl.sh
```

国内安装将wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-github.sh  换成   wget https://github.com/jinghunsanzu/ARL-set/releases/download/ARL/setup-arl-cn.sh
