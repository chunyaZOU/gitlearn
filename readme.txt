Git 常用命令
git init 初始化一个版本库
git add name.txt 添加一个文件
git commit -m"message content" 提交一次内容（执行此命令，需先执行git add命令）
git log 提交日志（该版本之前的提交，含该版本）
git reflog 提交日志（全部版本）
git log --pretty=oneline提交日志（单行只显示commit id）
git reset --hard commitId（回到commitId版本）