1，我fork了一个同事的项目A到我个人账户下，称为项目B。后来同事修改了一些信息，我需要将修改的信息同步到我账户下的项目B。

#添加项目A的远程仓库地址到upstream
git remote add upstream <你朋友项目A的仓库地址>

#把项目A的更新来到本地的upstream里
git fetch upstream

#切换到你自己想要merge的分支，这里我用举例：master
git checkout master

#merge项目A的更新到你的branch
git merge upstream/master