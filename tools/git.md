# Git

バージョン版本　プロジェクト项目　ローカル本地　クローン克隆　リポジトリ仓库 オープンソース开源 クラウド云
Git 是一个开源的分布式版本控制系统
Git は分散バージョン管理システムであり、プロジェクトのローカル クローンが完全なバージョン管理リポジトリであることを意味します。

[中文教程](https://www.runoob.com/git/git-tutorial.html)

## 1.下载安装配置

Linux,Mac,Windows
安装包 源代码ソースコード 命令 命令行工具 图形界面
环境变量 默认目录 本地版本库 远程版本库

homebrew
'
git/git-gui
brew install git
'
全局
git config --global user.name 'username'
git config --global user.email 'useremail'
git config --global core.editor 'code --wait'
git config --global merge.tool vimdiff
git config --list
git config user.name

生成SSH密钥
ssh-keygen -t rsa -b 4096 -C 'useremail'
git --version

## 2.工作流程

1.克隆仓库
git clone https://github.com/username/repo.git
cd repo
2.创建新分支
git checkout -b new-feature
3.工作目录,在工作区编辑,添加或删除
4.把文件修改添加到暂存区
git add filename
5.提交更改
git commit -m ‘提交信息’
6.从远程仓库拉取最新版本
git pull origin(远程名) main(分支名)
7.推送更改
git push origin main
8.创建pull request,评审代码,合并代码
9.合并更改
git checkout main
git pull origin main
git merge new-feature
10.删除分支
git branch -d new-feature
git push origin --delete new-feature
常用命令
查看暂存区
git status
查看提交记录
git log
比较工作区和暂存区之间的差异
git diff
比较暂存区和最后一次提交提交之间的差异
git diff --cached
获取远程仓库更新
git fetch origin branch-name
git merge origin/branch-name
编辑配置文件
git config -e
git config -e --global

## 3.创建仓库
初始化
mkdir my-project
cd my-project
git init
git init my-project
git clone repo
git clone repo my-repo

