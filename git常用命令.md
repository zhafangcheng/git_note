# git常用命令
## git config
用法：git config -global user.name"[your name]"
用法：git config -global user.email"[your email address]"
这两个命令分别设置提交代码的用户名和电子邮件地址。
## git init
用法：git init
该命令可以用于创建一个新的代码库
## git clone
用法：git clone [url]
该命令可以通过制定的URL获取一个代码库
## git add
用法：git add [file]
该命令可以将一个文件添加到stage【暂存区】
用法：git add *
该命令可以将多个文件添加到stage【暂存区】
用法：git add .
该命令将所有文件添加到stage【暂存区】
## git commit
用法：git commit -m "[可以记录小节/类似提交备注]"
该命令可以在版本历史记录中永久记录文件
用法：git commit -a
该命令是将提交git add 命令添加的所有文件，病提交git add命令之后有所更改的所有文件
## git diff
用法： git diff
该命令可以显示尚未添加到stage的文件的变更
用法：git diff -staged
该命令可以显示添加到stage的文件与最新版本之间的差异
用法：git diff [first branch] [second branch]
## git reset
用法：git reset [file]
该命令可以将stade【暂存区】中撤出制定的文件，但可以保留文件的内容
用法：git reset[commit]
该命令可以撤销制定提交之后的所有提交，病在本地保留变更
用法：git rest -hard [ commit]
该命令将丢弃所有的历史记录，并回滚到指定的提交
## git status
用法：git status
该命令将会显示所有需要提交的文件
## git rm
用法： git rm [file]
该命令将会删除工作目录中的文件，并将删除动作添加到stage
##  git log
用法： git log
该命令可以用于显示当前分支的版本历史记录
用法：git log -follow [file]
该命令可以用于显示某个文件的版本历史记录，包括文件的重命名
## git show 
用法：git show [commit]
该命令将会显示提交的元数据以及内容变更 
## git tag
用法：git tag [commitID]
该命令可以给制定的提交添加地址
## git branch
用法：git branch
该命令将会显示当前代码库中所有的本地分支
用法：git branch [branch name]
该命令将创建一个分支
用法：git branch -d [branch name]
该命令将会删除置顶的分支
## git checkout
用法：git checkout [branch name]
该命令可以切换分支
用法：git checkout -b [branch name]
该命令将会创建一个分支，并且切换到该新分支上
## git merge
用法：git merge [branch name]
该命令可以将置顶分支的历史记录合并到当前分支
## git remote
用法：git remote add [variable name] [Remote Server Link]
该命令会将本地的代码库连接到远程服务器
## git push
用法：git push [variable name] master
该命令可以将主分支上提交的变更发送到远程代码库
用法：git push [variable name] [branch]
该命令可以将指定分支上的提交发送到远程代码库
用法：git push –all [variable name]
该命令可以将所有分支发送到远程代码库
用法：git push [variable name] :[branch name]
该命令可以删除远程代码库上的一个分支
## git pull
用法：git pull [Repository Link]
该命令将获取远程服务器上的变更，并合并到你的工作目录
## git stash
用法：git stash save
该命令将临时保存所有修改的文件
用法：git stash pop
该命令将恢复最近一次stash(储藏)的文件
用法：git stash list
该命令将显示stash的所有变更
用法：git stash drop
该命令将丢弃最近一次stash的变更
