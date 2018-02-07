## 初始化Git仓库基础指令

`git-init` 旨在帮助第一次使用git的用户熟悉 `git init`、`git config`、`git clone`、`git add`、`git commit`、`git remote`、`git push` 等常用命令的简单用法，下面开始吧。

##### Git 全局设置

`git config --global user.name "王睿"`

`git config --global user.email "nihaorz@qq.com"`

##### 创建新版本库

`git clone git@172.16.101.190:nihaorz/git-init.git`

`cd git-command-study`

`touch README.md`

`git add README.md`

`git commit -m "add README"`

`git push -u origin master`

##### 已存在的文件夹

`cd existing_folder`

`git init`

`git remote add origin git@172.16.101.190:nihaorz/git-init.git`

`git add .`

`git commit -m "Initial commit"`

`git push -u origin master`

##### 已存在的 Git 版本库

`cd existing_repo`

`git remote rename origin old-origin`

`git remote add origin git@172.16.101.190:nihaorz/git-init.git`

`git push -u origin --all`

`git push -u origin --tags`