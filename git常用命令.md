1，我fork了一个项目A到我个人账户下，称为项目B。后来同事修改了一些信息，我需要将修改的信息同步到我账户下的项目B。

#添加项目A的远程仓库地址到upstream

git remote add upstream <项目A的仓库地址>

#把项目A的更新拉到本地的upstream里

git fetch upstream

#切换到你自己想要merge的分支，这里我用举例：master

git checkout master

#merge项目A的更新到你的branch

git merge upstream/master


2，如何在git中删除指定的文件和目录

#拉取远程的Repo到本地（如果已经在本地，可以略过） 

git clone xxxxxx

#在本地仓库删除文件 

git rm 我的文件

#在本地仓库删除文件夹 

git rm -r 我的文件夹/

#此处-r表示递归所有子目录，如果你要删除的，是空的文件夹，此处可以不用带上-r。强制更新可以带上-f

#提交代码 

git commit -m"我的修改"

#推送到远程仓库（比如GitHub） 

git push origin xxxxxx