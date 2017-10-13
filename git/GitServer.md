Git服务器搭建
=== 

1.建立用户

    $ groupadd git 
    $ adduser git -g git

>将/bin/bash替换成git-shell的路径
>可以通过#-> which git-shell来查看git-shell所在路径
>将/home/用户名称替换成/home/组目录名称

2.创建证书登录
 
    $ cd /home/git/
    $ mkdir .ssh
    $ chmod 700 .ssh
    $ touch .ssh/authorized_keys
    $ chmod 600 .ssh/authorized_keys

3.sshd相关设置问题:

    $ vim /etc/ssh/sshd_config

>RSAAuthentication yes            #开启RSA认证功能
>PubkeyAuthentication yes      #开启公匙认证 
>StricModes no                           

4.初始化Git仓库

    $ cd /home
    $ mkdir gitrepo
    $ chown git:git gitrepo/
    $ cd gitrepo

    $ git init --bare runoob.git
    $ chown -R git:git runoob.git
