# daily

此文件用于记录日常问题

## Git

1. 先网上下载 git
2. git 初次使用时，需要先配置一下
   git config --global user.name 'username'
   git config --global user.email 'email'

   username **标识提交者身份，可以在本地仓库提交记录中看到。和远程代码托管平台账号名并不互相影响**
   user.email 会在你将本地仓库提交给远程代码托管平台（如 github）时，**平台会根据提交记录的 email 匹配到你的账号，方便其他人识别你**

3. git 基本概念
   工作区 人们编写代码的区域
   暂存区 人们暂存代码的区域，如我写好一个功能，暂时将功能代码储存的区域

   分支 人们可以在不影响主代码的影响下，独立的进行代码开发。可以理解为基于主代码上的自己更改后的代码版本
   仓库 **包含项目所有文件，以及所有文件更改历史记录的集合**，分为本地仓库和远程仓库，本地仓库存储在本地计算机内，远程仓库存储在服务器上
   合并 将一个分支的代码集成到另一个分支的操作
   远程 **与本地仓库关联的远程仓库**，通过配置远程仓库，开发者可以将本地代码提交到远程仓库中，或者从远程仓库中拉取最新的代码到本地仓库

4. git 基本操作
   **git add .**: 将更改的代码添加到暂存区 <br>
   **git restore 'file'**: 移除工作区的代码 <br>
   **git restore --staged 'file'**: 将指定文件从暂存区移除 <br>
   **git commit -m 'message'**: 将暂存区的代码添加到当前的分支 <br>
   **git clone 'repository name'**: 克隆远程仓库的代码到本地 <br>
   **git branch 'branch name'**: 创建一个新分支 <br>
   **git switch 'branch name'**: 切换到另一个分支 <br>
   **git switch -c 'branch name'**: 创建一个新分支，并且切换到新分支 <br>
   **git merge 'branch name'**: 合并分支 <br>
   **git remote add origin 'repository address'**: 关联远程仓库，用于获取远程最新代码，或者推送本地代码到远程仓库 <br>
   **git push --set-upstream origin 'branch name'**: 将本地分支推送到远程分支，并关联远程分支 <br>

## 好用的 Vscode 插件

1. **Auto Import - ES6, TS, JSX, TSX**: 自动查找、解析所有可用的导入，并提供代码操作和代码补全功能。适用于 JavaScript（ES6）和 TypeScript（TS）<br>
2. **Auto Rename Tag**: 自动重命名配对的 HTML/XML 标签 <br>
3. **Chinese (Simplified) (简体中文) Language Pack for Visual Studio Code**: 此中文（简体）语言包为 VS Code 提供本地化界面 <br>
4. **Code Runner**: 运行多种语言的代码片段或代码文件 <br>
5. **ES7 React/Redux/GraphQL/React-Native snippets**: 这个扩展为你提供适用于 VS Code 的、具备 Babel 插件特性、采用 ES7 语法的 JavaScript 以及 React/Redux 代码片段 <br>
6. **ESLint**: 代码检查,代码风格统一,自动修复 <br>
7. **Prettier - Code formatter**: Prettier 是一个有主见（opinionated）的代码格式化工具，“有主见” 意味着它有一套内置的、固定的代码格式化规则，开发者无需花费大量时间去自定义各种细微的格式规范，它会按照自己认为最佳的方式来格式化代码。 <br>
8. **Live Server**: 启动一个具备实时重新加载功能的本地开发服务器，用于静态和动态页面。 <br>
9. **Material Icon Theme**: 适用于 Visual Studio Code 的 Material Design（材质设计）图标 <br>
10. **Path Autocomplete**: 为 Visual Studio Code 和 Web 版 Visual Studio Code 提供路径补全功能。<br>
11. **vscode-styled-components**: 为 styled-components 提供语法高亮显示 <br>
