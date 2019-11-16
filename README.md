# project-git
a git demo Project

## 创建ssh在用户文件夹下
- ssh-keygen -t rsa 
- 找到 .ssh/id_rsa.pub 的公钥 添加到github

## 设置用户名和邮箱
- git config --global user.email 6@gmail.com
- git config --global user.name ZeroShiro
- git config -l  查看

## 克隆仓库
- git clone github的/地址

## 提交暂存区
- git add .\index.html .\README.md  (暂存区Area)
- git add .  (添加当前全部)
- git status (查看状态)

## 创建分支
- git branch             查看分支
- git branch name        创建分支
- git branch -d name     删除分支
- git checkout           切换分支
- git checkout -b name-1 创建并进入
- git merge name         合并分支

## 查看版本
- git log 
- git reflog

## 撤销
- git checkout -- name  撤销工作区
- git reset HEAD name   撤销暂存区

## 版本回退
- git reset --hard HEAD^     (一个^表示一个版本)
- git reset --hard HEAD~1   
- git reset --(hard | mixed(默认) | soft)  HEAD~(num) or commit(id)

## 版本合并
- git rebase -i HEAD~num 最近提交x个commit

## 差异比较
- git diff                         比较工作区和暂存区
- git diff HEAD                    比较工作区和本地版本库中最近一次commit的内容
- git diff --cached                比较暂存区和本地版本库中的最近一次commit内容
- git diff <commit-id> <commit-id> 比较2个commit的差异

## 提交
-  一个版本一个commit -m->message
-  git commit -m '本地仓库一' 传本地仓库
-  git push  origin master   传远程仓库
-  git push -u origin master 指定origin为默认主机 
-  git pull origin master 拉代码


