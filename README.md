### Git介绍

`Git`是Linus于2005年开发的一个`开源`,`分布式`的版本控制系统。

Git 开发起初，他们设定的目标是：<br />
* 速度 
* 简单的设计 
* 对非线性开发模式的强力支持（允许上千个并行开发的分支） 
* 完全分布式 
* 有能力高效管理类似 Linux 内核一样的超大规模项目（速度和数据量）

#### 提供代码仓库服务的网站有：
国外：
* Github
* BitKeeper
* BitBucket

国内：
* OsChina 
* taoCode
* Codding


#### Git简介

Git是版本控制管理工具，作者Linus

git log 命令选项

![git-log.png](https://github.com/zaifeng/Git/blob/master/images/git-log.png "option words")


```git status -s``` 可以查看系统那些文件做了那些修改

例如：
```
$git status -s
M hello.md

$git diff 用于查看difference,显示的格式正是Unix通用的diff格式

$git diff 无参数情况，表示工作区和索引区对比

$git diff --cached 表示索引区和版本控制区对比

用git diff HEAD -- readme.txt命令可以查看工作区和版本库里面最新版本的区别
```

h.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  ``git config --global push.default matching``

To squelch this message and adopt the new behavior now, use:

  ``git config --global push.default simple``

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    ``git push --set-upstream origin master``

``--set-upstream`` 效果等同于 -u ,只需与远程绑定一次，以后即可使用简略命令

合并分支时，加上``--no-ff``参数就可以用普通模式合并
--no-ff 选项可以看出log的图形效果

```
git reset -- file 用于撤销暂存区的修改
git reset HEAD -- file 用于撤销暂存+工作区的修改
```