#### 为什么需要Git

平时的文本编辑器编辑 没有保存功能 可能一次死机 之前写的文件或者内容都不见了
所以需要一个软件来统筹我们的文本记录

#### Git的优点

分支管理

本地仓库

保持的是文件的差异 比较轻量


#### Git基础

本地仓库 远程仓库

git init初始化 生成.git文件

新建的文件 没有加入暂存区  纳入版本控制

git add . 添加文件夹下所有文件 放入暂存区
 
git commit -m 'xxx' 提交一个记录 放入本地仓库

会通过类似md5的方式生成一个commit id 例如 594a49a

git remote add origin https://github.com/MrCodeSniper/GitDev.git 将本地仓库与远程仓库绑定

git push -u origin master 将本地仓库内容推送到远端master分支

git pull 从远端拉代码下来 

git stash 将本地的未提交的修改 生成一个Stash可暂存起来

git pop 将stash的修改恢复

git log 可以查看提交的记录信息



#### 冲突处理

<<<<<<<<<HEAD  (HEAD指向的是我们本地的修改)
ABCDEFG
========
ABCEFGD
>>>>>>>>> B5CDFDFSCDSCSDFSFSF (记录对应的是对方的修改)

## CH


解决冲突的时候 遇到别人提交的代码 不要轻易的删除 要问清楚是做什么的 

1.如果不影响你的代码

ABCDEFG
ABCEFGD 保留双方代码

2.如果影响你的代码

将代码修改为正确的形式






