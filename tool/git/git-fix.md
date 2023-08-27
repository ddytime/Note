### git将密码替换成token
1.生成token
- 打开Github，在个人设置页面，找到【Setting】，然后打开找到【Devloper Settting】然后，选择个人访问令牌【Personal access tokens】，然后选中生成令牌【Generate new token】
- 要使用token从命令行访问仓库，请选择repo
- 要使用token从命令行删除仓库，请选择delete_repo
- 其他根据需要进行勾选

2.生成token后，使用token提交代码
git remote set-url origin https://<your_token>@github.com/<USERNAME>/<REPO>.git
- <your_token>:换成你的token
- <USERNAME>:是你的git用户名
- <REPO>:是你的仓库名称

