# git 的进阶操作

git is free software

git is free software distributed under the GPL

git diff 与上一次提交不同的地方
git log 由近到远的提交日志
git log --pretty=oneline 提交代码的版本号

git 支持分布式提交：多人同时协作

git reset --hard HEAD 版本回退 HEAD 为当前版本

git reset --hard HEAD~2 暂存区回退两个版本

git reset --hard 版本号名称 暂存区回到固定版本号

git reset --soft HEAD^ 文件名 撤销刚刚的那次 commit,撤回缓存区

git relog 查看历史日志的命令

ls -ah 当前目录的隐藏文件

git commit 将暂存区的代码提交到当前分支上

远程仓库里只有最新版本

暂存区保有所有的版本，但是一旦将 commit 本地主分支上的代码 push 出去之后，master 分支将会变得很干净，无法回退

git 的优点

1. git 只跟踪文件中单词修改的文字，而非文件

2. 分部式可以使多人协作

工作流：通过 git add . 将修改的代码推入暂存区，用 git commit 命令推入 master 主分支，再用 push 命令推入远程代码

修改文字 a--->git add .------>再次修改文字 ab------->git commit -m ""-------->push
-------------存入一次更改------------------------>存入 master 分支 a ---------->推入远程仓库  
------------------------------------------------------ 清空
