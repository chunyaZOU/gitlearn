#### Git Learn
##### Git 常用命令
1. git init 初始化一个版本库
2. git add name.txt 添加一个文件修改到暂存区
3. git commit -m"message content" 提交一次内容修改
git中暂存区是一个非常重要的概念，可以多次修改文件，并将修改添加到暂存区，一次性commit所有修改到当前分支。没有被add到暂存区的修改不会被commit
4. git log 提交日志（该版本之前的提交，含该版本）
5. git reflog 提交日志（全部版本）
6. git log --pretty=oneline提交日志（单行只显示commit id）
7. git reset --hard commitId（回到commitId版本）
8. git checkout -- readme.txt 将工作区的修改全部撤销，--很重要 ，否则就变成了切换分支的命令
8.1 修改还没有添加到暂存区，撤销修改就回到和版本库一模一样状态
8.2 修改已经添加到暂存区，又做了修改，再撤销修改就回到添加暂存区后的状态
就是让文件回到最近一次的commit或add状态
9.
