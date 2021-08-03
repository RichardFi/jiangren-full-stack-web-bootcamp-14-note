# 05-Git

## Git 课堂笔记

### 1. Git version control
- 可以撤销改动或回滚版本
- 合作
- 备份

### 2. Git分布式开发 distributed
- 每个developer都有所有的source code
- 无中央服务器
- 不只是开源软件，公司也普遍使用分布式

### 3. Git和Github
- Github提供一个平台，将项目的repo托管在Github上，developers可以在github取得source code
- Github已经被微软收购

### 4. Git global setup
- `git config --global user.name "<Your-Full-Name>"`
- `git config --global user.email "<Your-Email-Address>"`
- `git config --global color.ui auto`
- `git config --global core.editor "code --wait"`

### 5. 初始化一个git repo
- `git init`
- `git clone` clone一个已存在的repo

### 6. Git的工作原理
- `git add ./index.html` 添加文件到stage状态
- `git commit -m 'add index.html to project'` commit添加的文件

### 7. Git stash暂存当前进度

### 8. Git message要有意义

### 9. Git undo changes
- `git checkout .` checkout当前目录，对当前目录从repo中复原
- `git clean` clean当前目录，会删除文件
- `git revert` 用一个新的commit回滚，这个操作是可追溯的
- `git reset` 从历史记录种删除commit，更加危险，看不到操作，一般在公司中不被允许

### 10. Branching
- 主branch为 master 或者 main
- `git branch` 当前branch
- `git branch -d` 删除branch
- `git checkout -b`
- `<type>/<ticket-number>-<title>`
- merge branch 将自己的branch与master merge

### 11. merge conflict管理
- 要按master branch在自己的branch上进行

### 12. 远程协作
- `git clone` Connect to remote repo
- `git branch -u <name>/<branch>` Set up tracking branch
- `git upload` `git pull` 更新本地repo
- `git push` 用本地更新远程repo

### 13. pull request
- owner在review后可以选择merge pull request

### 14. squash and merge
- 压缩merge，将很多对于同一个feature的commit整合后进行merge，使这个行为更好理解
- 可能引起一些问题，例如不方便revert

### 15. Rebase
- 不使用merge而使用rebase
- 使项目的修改历史更清楚

### 作业
- 把github的url发给tutor看