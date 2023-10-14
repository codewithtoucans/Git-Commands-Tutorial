# git commands tutorial
pratice and enjoy yourself 🥳.

{{TOC}}

## git basic command

|:--|:--|
|  git --version | 查看git版本 |
|  git init                |初始化本地项目库                      |
|  git status              |查看文件状态                          |
|  git add [filename]      |提交文件到暂存区                      |
|  git add .               |提交所有文件到暂存区                  |
|  git commit -m '[message]' |提交文件并附带信息                    |
|  git ls-files            |展示本地仓库中提交的文件              |
|  git rm [filename]       |将文件从本地仓库中删除                |
|  git mv [old filename] [new filename] |本地仓库中文件重命名|
|  git log                 |展示提交历史                          |
|  git log --oneline       |展示提交历史,提交信息展示在一行       |
|  git reflog                     | 展示本地仓库历史修改内容|
|  git checkout -- [filename]        |  丢弃未暂存文件中所做的修改(也可以省略--)                   |
|  git checkout .                    |  丢弃所有未暂存文件中所做的修改                             |
|  git restore [filename]            |  丢弃未暂存文件中所做的修改                                 |
|  git restore --staged [filename]   |  将暂存区的文件移除暂存区                                   |
|  git reset [filename]              |  将暂存区的文件移除暂存区                                   |
|  git clean -dn                     |  列出所有要删除的未跟踪的文件                               |
|  git clean -df                     |  删除未跟踪的文件                                           |
|  git reset HEAD~[number]           |  将HEAD后退number个版本，并将之间提交的文件变为未跟踪状态   |
|  git reset --soft HEAD~[number]    |  将HEAD后退number个版本，并将之间提交的文件移置暂存区       |
|  git reset --hard HEAD~[number]    |  将HEAD后退number个版本，并将之间提交的文件全部删除         |
  
   
## git branch command

|:--|:--|
|   git branch                 |展示本地分支                         |
|   git branch [branch name]   |新建一个分支                         |
|   git branch -d [branch name]|删除一个分支                         |
|   git branch -D [branch name]|强制删除一个分支                     |
|   git branch -a              |展示所有分支                         |
|   git branch -r              |展示远程分支                         |
|   git branch -vv             |展示本地跟踪分支和链接远程分支信息   |
|   git checkout [branch name]    | 切换分支                      |
|   git switch [branch name]      | 切换分支                      |
|   git checkout -b [branch name] | 创建一个新分支并切换到该分支  |
|   git switch -c [branch name]   | 创建一个新分支并切换到该分支  |


## git stash command

|:--|:--|
|   git stash                     |将未提交文件的所有修改部分暂存起来|
|   git stash apply               |将暂存的部分还原回文件            |
|   git stash list                |展示暂存修改列表                  |
|   git stash pop                 |将暂存的部分还原回文件            |
|   git stash apply [number]      |指定还原序号暂存部分的文件        |
|   git stash pop [number]        |指定还原序号暂存部分的文件        |
|   git stash drop [number]       |丢弃暂存文件的修改部分            |
|   git stash push -m "[message]' |附加提示信息将修改部分暂存起来    |
|   git stash clear               |丢弃所有暂存文件的修改部分        |
 
## git merge command

|:--|:--|
|   git merge [branch name]        | 将其他分支合并到当前分支|
|   git rebase [branch name]       | 变基合并分支            |
|   git check-pick [command hash]  | 将指定提交合并到当前分支|

## git tag command

|:--|:--|
|   git tag                                | 展示标签列表            |
|   git tag [tag name] [command hash]      | 给某个提交设置tag       |
|   git show [tag name]                    | 展示某个tag信息         |
|   git checkout [tag name]                | HEAD切换到tag           |
|   git tag -d [tag name]                  | 删除tag标签             |
|   git tag -a [tag name] -m '[message]'   | 给当前头打tag并附加信息 |

## git remote command

|:--|:--|
|   git remote -v                                          | 展示远程仓库url                                      |
|   git remote add origin [url]                            | 添加远程仓库地址                                     |
|   git push origin [banch name]                           | 本地仓库推送到远程分支上(分支不存在，远程创建新的)   |
|   git ls-remote                                          | 展示远程分支信息                                     |
|   git fetch                                              | 更新远程仓库信息到远程跟踪分支                       |
|   git pull origin [branch name]                          | 拉取远程分支并合并到当前分支上                       |
|   git branch --track [branch name] [remote branch name]  | 创建本地跟踪分支链接远程分支                         |
|   git remote show origin                                 | 查看远程仓库分支信息                                 |
|   git clone [url]                                        | 克隆远程仓库到本地                                   |
|   git clone [url] [project name]                         | 克隆远程仓库到本地并修改目录名                       |
|   git push -u origin [branch name]                       | 推送项目到远程分支并创建本地跟踪分支                 |
|   git push origin [branch name]                          | 推送项目到远程分支                                   |
|   git push origin --delete [remote branch name]          | 删除远程仓库分支                                     |
|   git push --force origin [branch name]                  | 强行推送项目到分支                                   |
|   git remote set-url origin [url]                        | 修改远程地址                                         |
 
 
