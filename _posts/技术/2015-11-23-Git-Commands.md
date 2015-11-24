---
layout: post
title: Git常用命令速查表
category: 工具
tags: git
---

master:默认开发分支
origin:默认远程版本库

### 创建版本库

```
$ git clone <url>   #克隆远程版本库
$ git init          #初始化本地版本库
```

### 修改和提交

```
$ git status        #查看状态
$ git diff          #查看变更内容
$ git add .         #跟踪所有改动过的文件
$ git add <file>    #跟踪指定的文件
$ git mv <old><new> #文件改名
$ git rm<file>      #删除文件
$ git rm --cached<file>            #停止跟踪文件但不删除
$ git commit -m "commit messages"  #提交所有更新过的文件
$ git commit --amend               #修改最后一次改动
```

### 查看提交历史

```
$ git log                    #查看提交历史
$ git log -p <file>          #查看指定文件的提交历史
$ git blame <file>           #以列表方式查看指定文件的提交历史
```

### 撤销

```
$ git reset --hard HEAD      #撤销工作目录中所有未提交文件的修改内容
$ git checkout HEAD <file>   #撤销指定的未提交文件的修改内容
$ git revert <commit>        #撤销指定的提交
$ git log --before="1 days"  #退回到之前1天的版本 
```

### 远程操作

```
$ git remote -v                   #查看远程版本库信息
$ git remote show <remote>        #查看指定远程版本库信息
$ git remote add <remote> <url>   #添加远程版本库
$ git fetch <remote>              #从远程库获取代码
$ git pull <remote> <branch>      #下载代码及快速合并
$ git push <remote> <branch>      #上传代码及快速合并
$ git push <remote> :<branch/tag-name>  #删除远程分支或标签
$ git push --tags                       #上传所有标签
```



### 资料链接
1. [Try Git](https://try.github.io/levels/1/challenges/1)
2. [Git教程——廖雪峰官网](http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/)



