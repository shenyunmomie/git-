[TOC]

# git入门教程

此为使用git相关功能的教程
git是一款**分布式版本控制系统**

## Git核心概念
+ Workspace： 工作区，就是你平时存放项目代码的地方

+ Index / Stage： 暂存区，用于临时存放你的改动，事实上它只是一个文件，保存即将提交到文件列表信息

+ Repository： 仓库区（或版本库），就是安全存放数据的位置，这里面有你提交到所有版本的数据。其中HEAD指向最新放入仓库的版本

+ Remote： 远程仓库，托管代码的服务器，可以简单的认为是你项目组中的一台电脑用于远程数据交换
![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/2ece9523-dcf9-4926-bed3-9df53f6ce6de)
![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/4acafcba-7178-4900-aa2c-36c45bf1a59e)

在初始化git版本库之后会生成一个隐藏的文件 .git ，可以将该文件理解为git的版本库 repository，而我们自己建立的项目文件夹即工作区 working directory ,在.git 文件夹里面还有很多文件，其中有一个index 文件 就是暂存区也可以叫做 stage ,git还为我们自动生成了一个分支master以及指向该分支的指针head

![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/a866d62c-3126-4e6a-96b7-8bf14c1f6cf9)

从图中可以看出来respository包括分支master和stage, working diretory 可以理解为我们打开开发环境如eclipse，里面的内容即工作区的内容，在工作区里面有的代码以及配置文件等我们需要提交到版本库里面，最终是到了分支master上面，暂存区只是一个临时保存修改文件的地方。

 **比喻：**

这就像是搭积木，要搭一个村庄，工作区就是桌子，我们从零件开始一个个搭房子，搭好一个房子后，将其转移到暂存区保存，因为桌子上不安全，会疏忽大意毁掉房子。

搭好所有房子后，全部放到暂存区组合，就完成了村子(一个版本)，这时候能运行就可以提交到仓库区保存，这是第一个版本。

如果不满意需要修改，从仓库区中拉取，到暂存区和工作区，在工作区一个房子一个房子的修改，然后提交暂存区，如果这时觉得某个房子还是不修改好看，则直接回滚。

（未完待改）

## Git工作流程

+ 从远程仓库中克隆 Git 资源作为本地仓库；
+ 从本地仓库中checkout代码然后进行代码修改；
+ 在提交本地仓库前先将代码提交到暂存区；
+ 提交修改，提交到本地仓库；本地仓库中保存修改的各个历史版本；
+ 在需要和团队成员共享代码时，可以将修改代码push到远程仓库。
  ![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/b26afd68-351a-43f2-9911-0fc1084326ba)
  ![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/932cd862-8d52-40bf-9f46-0fcb09be5b48)

## git配置
设置用户名称和 email 地址。这是非常重要的，因为每次 Git 提交都会使用用户信息。

```python
git config
git config --global user.name shenyunmomie
git config --global user.email sw18732566535@gmail.com
```

+ --local（默认高优先级）：只会影响到本地仓库
+ --global(中优先级）：只会影响到当前用户的git仓库
+ --system（低优先级）:影响到全系统git仓库

## git常用命令

### git add

测试

# gitkraken图形化界面

