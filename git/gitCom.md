Git 学习笔记
============

1.安装

  Linux
    sudo apt-get install git

  Mac
    homebrew
      https://brew.sh/index_zh-cn.html

    xcode
      选择菜单“Xcode”->“Preferences”，在弹出窗口中找到“Downloads”，选择“Command Line Tools”，点“Install”

  Windows
    https://git-for-windows.github.io

2 使用
  

  设置

    设置用户名／邮箱
      git config --global user.name "Your Name"
      git config --global user.email "email@example.com"

    创建版本库
      git init

  远程仓库操作

    建立密钥
      ssh-keygen -t rsa -C "youname@xxx.com"

    在本地目录下关联远程repository
      git remote add origin git@github.com:git_username/repository_name.git

    取消本地目录下关联的远程库
      git remote remove origin

    克隆远程仓库
      git clone git@github.com:username/repositoryname.git

  基本操作

    状态
      git status [-s]

    工作区 -> 暂存区
      git add

    暂存区 -> 版本库
      git commit -m "message"

    提交日志
      git log [--pretty=oneline]

    命令日志
      git reflog

  三区比较差异

    工作区文件与暂存区的不同
      git diff -- [filename]

    工作区和版本库的不同
      git diff HEAD -- [filename]

    暂存区和版本库的不同
      git diff --cached -- [filename]

  版本控制

    回退到上一个版本
      git reset --hard HEAD^

    回退到某一版本,重置暂存区和工作区
      git reset --hard <commitId>

    回退到某一版本,重置暂存区
      git reset --mixed <commitId>

    回退到某一版本,之后的修改退回暂存区
      git reset --soft <commitId>

    回退到某一版本,并且作为一个新版本创建
      git revert <commitId>

    暂存区->工作区
      git checkout [-- file]

  分支操作

    查看分支
      git branch

    创建分支
      git branch <name>

    切换分支
      git checkout <name>

    创建+切换分支
      git checkout -b <name>

    合并某分支到当前分支
      git merge <name>

    删除分支
      git branch -d <name>




