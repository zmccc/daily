# daily
此文件用于记录日常问题

## Git
1. 先网上下载git
2. git初次使用时，需要先配置一下
    git config --global user.name 'username'
    git config --global user.email 'email'

    username __标识提交者身份，可以在本地仓库提交记录中看到。和远程代码托管平台账号名并不互相影响__
    user.email会在你将本地仓库提交给远程代码托管平台（如github）时，__平台会根据提交记录的email匹配到你的账号，方便其他人识别你__
3. git基本概念
    工作区   人们编写代码的区域
    暂存区   人们暂存代码的区域，如我写好一个功能，暂时将功能代码储存的区域

    分支     人们可以在不影响主代码的影响下，独立的进行代码开发。可以理解为基于主代码上的自己更改后的代码版本
    仓库     __包含项目所有文件，以及所有文件更改历史记录的集合__，分为本地仓库和远程仓库，本地仓库存储在本地计算机内，远程仓库存储在服务器上
    合并     将一个分支的代码集成到另一个分支的操作
    远程     __与本地仓库关联的远程仓库__，通过配置远程仓库，开发者可以将本地代码提交到远程仓库中，或者从远程仓库中拉取最新的代码到本地仓库
4. git基本操作
    __git add .__: 将更改的代码添加到暂存区
    __git restore 'file'__: 移除工作区的代码
    __git restore --staged 'file'__: 将指定文件从暂存区移除
    __git commit -m 'message'__: 将暂存区的代码添加到当前的分支
    __git clone 'repository name'__: 克隆远程仓库的代码到本地
    __git branch 'branch name'__: 创建一个新分支
    __git switch 'branch name'__: 切换到另一个分支
    __git switch -c 'branch name'__: 创建一个新分支，并且切换到新分支
    __git merge 'branch name'__: 合并分支
    __git remote add origin 'repository address'__: 关联远程仓库，用于获取远程最新代码，或者推送本地代码到远程仓库