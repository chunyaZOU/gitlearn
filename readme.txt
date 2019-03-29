Git 常用命令
git init 初始化一个版本库
git add name.txt 添加一个文件修改到暂存区
git commit -m"message content" 提交一次内容修改
git中暂存区是一个非常重要的概念，可以多次修改文件，并将修改添加到暂存区，一次性commit所有修改到当前分支
git log 提交日志（该版本之前的提交，含该版本）
git reflog 提交日志（全部版本）
git log --pretty=oneline提交日志（单行只显示commit id）
git reset --hard commitId（回到commitId版本）