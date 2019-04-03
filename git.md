| 目标                                       | 命令                                  |
| ------------------------------------------ | ------------------------------------- |
| 创建仓库                                   | git init                              |
| 与远程仓库建立联系                         | git remote add <name> <远程仓库 url>  |
| 首次上传到远程仓库                         | git push --set-upstream <name> master |
| 添加到缓存区                               | git add                               |
| 从缓存区删除                               | git rm --cache <fileName>             |
| 从远程仓库下载代码                         | git clone <远程仓库 url>              |
| 远程仓库更新后更新本地仓库                 | git pull                              |
| 查看远程仓库                               | git remote -v                         |
| 删除本地与远程仓库的联系                   | git remote rm <name>                  |
| 将本地 name1 分支提交到远程仓库 name2 分支 | git push <name> <name1>:<name2>       |
| 创建远程分支并推到远程                     | git push <name> <branch-name>         |
| 查看本地分支                               | git branch                            |
| 查看远程分支                               | git branch -r                         |
| 创建本地分支                               | git branch <branch-name>              |
| 切换分支                                   | git checkout <branch-name>            |
| 删除本地分支                               | git branch -d <branch-name>           |
| 删除远程分支                               | git push origin :heads/<branch-name>  |

**情景一---->撤销**
把不想要的代码 commit 到本地仓库，还没有推到远程仓库

#### 撤回对某个文件的 git add 操作

git reset HEAD <fileName>

#### 文件修改但是没有执行 git add

git checkout -- <fileName>

#### 合并两次 git commit 操作

git commit --amend -m 'text'

#### 撤回某一次git commit 操作----->回滚
git rest 
**情景二**
远程仓库的代码有问题，需要还原这次提交的代码
**情景三**
刚刚推到远程仓库的代码有问题，需要彻底撤回
