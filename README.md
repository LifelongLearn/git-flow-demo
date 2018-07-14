# git-flow-demo
体验一下git-flow的功能


# git-flow-demo
体验一下git-flow的功能

[https://www.git-tower.com/learn/git/ebook/cn/command-line/advanced-topics/git-flow](https://www.git-tower.com/learn/git/ebook/cn/command-line/advanced-topics/git-flow)

所有分支

master
develop
feature
bugfix
release
hotfix
support
prefix


# 步骤

## 1.开发新功能

为新功能创建分支
```cmd
git flow feature start [分支名]
```
把新功能合并到develop分支
```cmd
git flow feature finish [分支名]
```

有疑问查看 
```cmd
git flow feature help
```


```cmd
usage: git flow feature [list]
   or: git flow feature start
   or: git flow feature finish
   or: git flow feature publish
   or: git flow feature track
   or: git flow feature diff
   or: git flow feature rebase
   or: git flow feature checkout
   or: git flow feature pull
   or: git flow feature delete

    Manage your feature branches.
```


## 2.发布新功能

创建release（名称使用版本号，发布成功自动生成tag）
```cmd
git flow release start [版本号]
```

完成release（需要合并到develop和master分支上，写备注否则tag打不上去）
```cmd
git flow release finish [版本号]
```

## 3.快速修复HotFix

创建hotfix