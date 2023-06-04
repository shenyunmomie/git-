# git入门教程
此为使用git相关功能的教程
git是一款**分布式版本控制系统**
## Git工作流程
+ 从远程仓库中克隆 Git 资源作为本地仓库；
+ 从本地仓库中checkout代码然后进行代码修改；
+ 在提交本地仓库前先将代码提交到暂存区；
+ 提交修改，提交到本地仓库；本地仓库中保存修改的各个历史版本；
+ 在需要和团队成员共享代码时，可以将修改代码push到远程仓库。
![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/b26afd68-351a-43f2-9911-0fc1084326ba)
![image](https://github.com/shenyunmomie/git_teaching/assets/95114009/932cd862-8d52-40bf-9f46-0fcb09be5b48)
## Git核心概念
+ Workspace： 工作区，就是你平时存放项目代码的地方

+ Index / Stage： 暂存区，用于临时存放你的改动，事实上它只是一个文件，保存即将提交到文件列表信息

+ Repository： 仓库区（或版本库），就是安全存放数据的位置，这里面有你提交到所有版本的数据。其中HEAD指向最新放入仓库的版本

+ Remote： 远程仓库，托管代码的服务器，可以简单的认为是你项目组中的一台电脑用于远程数据交换


## fork分支


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



