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
就是让文件回到最近一次的commit或add状态，也可以用git reset命令回到上个版本
9. git rm file 删除文件，git中删除也是一个修改操作，记得commit到版本库
10. 远程仓库  
10.1. 可以直接克隆  
10.2. 可以创建一个空的远程仓库关联本地仓库：  
git remote add origin git@github.com:chunyaZOU/gitlearn.git
11. git push -u origin master 把本地仓库的所有内容推送到远程仓库  
第一次推送加上-u参数，不但可以把本地推送到远程，还可以将远程与本地关联
12. git clone xxxxxx 从远程克隆一个仓库
13. git checkout -b dev 创建并切换分支相当于git branch dev + git checkout dev两条组合
14. git branch 查看当前分支
15. git checkout branchName 切换分支  
16. git merge branchName 合并指定分支到当前分支
17. git branch -d branchName 删除指定分支
18. 合并：当git无法自动合并分支时，就必须首先解决冲突。解决冲突后，再提交，合并完成。
19. git log --graph 查看分支合并图
