# 代码之外的软技能

> Just for fun
> 本着不负责任的态度去学习
> 也就是本着 玩儿玩儿 的心态

## Markdown

### 将 Markdown 转成 Web PPT

https://github.com/fritx/markppt

0. 安装node环境（可以在cmd中输入 node -v 查看是否安装）
1. 执行 `npm install --global markppt`
2. 切换到要转换 PPT 的 Markdown 文件目录
3. 执行 `markppt md文件名`

## 版本管理

- 什么是版本管理

## SVN

### SVN 客户端基本操作流程

1. 通过 `checkout` 从服务器上把代码仓库下载下来
  - 只要指定了该操作，会在当前目录下生成一个隐藏文件 `.svn`
2. 然后客户端就可以在本地修改源代码了
3. 当修改了源代码，客户端要先把修改的文件通过 `add` 操作把文件添加到 待提交列表 中
  - 只有新建的文件需要手动 `add`
  - 对于 修改、更新、删除 都不需要手动 `add`
4. 接下来通过 `commit` 操作把 待提交列表中的项 commit 到远程仓库中
  - 注意：在提交之前，一定要记得先 update
  - 目的是为了看一下有没有冲突
  - 提交的时候，一定记得写 提交日志
5. 客户端可以通过 `update` 操作获取远程版本仓库中的最新版本

### 小组协作

```
其中一个人在自己的计算机上搭建一个 SVN 服务器（使用 VisualSVN搭建）
然后给其它小组成员创建账号
然后创建项目，给小组成员账号分配权限

小组成员通过 TortoiseSVN 客户端 操作远程仓库

注意：小组成员在 checkout 远程仓库地址的时候，SVN 服务器管理员要把
仓库的地址告诉小组成员

https://SVN服务器ip地址/svn/JD/
```

## Git

### 基本命令

- git clone 仓库地址
- git init 仓库名称
  + 只要执行了该命令，git 会帮你自动创建一个目录，然后在该目录下生成一个 `.git` 目录
- git statsu
  + 查看当前工作树的状态
- git add 文件名
  + 将操作的文件添加到 暂存区，待提交
- git commit -m "提交日志"
  + 上面这条命令表示将暂存区中的文件提交到本地仓库
  + 使用 git commit 的时候，最好告诉版本仓库，你这一次提交的作者是谁，邮箱是多少
- git log
  + 查看提交日志
- git config --global user.name "用户名"
- git config --global user.email "邮箱"
- git push
  + 将本地仓库推送到远程仓库

## Github

## 目标

1. 掌握Markdown的书写语法
2. 掌握版本管理控制的概念
3. 掌握 SVN 版本管理系统的基本使用
4. 掌握 Git 以及 Github 的基本使用
5. 掌握使用 hexo 部署个人博客到 Github
6. 掌握科学上网的几种方式
7. 掌握微信小程序的基本开发方式
