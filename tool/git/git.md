### git基本使用
1.创建本地仓库
- git init

2.将文件放到本地仓库中
- 在本地仓库中创建文件并修改内容
- git status查看本地仓库状态

3.将项目提交到暂缓区
- git add --all
- 提交后可以使用git status查看状态，确认文件都已经提交

4.提交到仓库
- git commit -m "提交信息"
- 使用git commit -a可以不用使用git add命令直接提交

5.将本地仓库和远端仓库关联
- 需要token git remote set-url origin https://<your_token>@github.com/<USERNAME>/<REPO>.git
- 不需要token git remote add origin https://.../*.git

6.上传代码
- git push -u origin master

### git工作流
![git工作流](../../images/git/git-process.png "git process")

### git工作区 暂缓区 版本区
- 工作区：就是你在电脑里能看到的目录
- 暂存区：英文叫 stage 或 index。一般存放在 .git 目录下的 index 文件（.git/index）中，所以我们把暂存区有时也叫作索引（index）
- 版本库：工作区有一个隐藏目录 .git，这个不算工作区，而是 Git 的版本库

### git基本操作
| 命令 | 说明 |
| :--- | :--- |
| git init | 初始化仓库 |
| git clone | 拷贝一份远程仓库，就是下载一个项目 |
| git add | 添加文件到暂缓区 |
| git status | 查看当前仓库状态，显示有变更的文件 |
| git diff | 比较文件的不同，暂缓区和工作区的差异 |
| git commit | 提交暂缓区到本地仓库 |
| git reset | 回退版本 |
| git rm | 将文件从暂缓区和工作区删除 |
| git mv | 移动文件或者重命名工作区文件 |