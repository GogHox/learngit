# git学习
1. `git init` : 将当前目录作为仓库
2. `git config --global user.name "name"`
   `git config --global user.email "email"`
	配置姓名和邮箱, `--global`代表配置所有的, 也可以只分别配置每个不同的 
3. `pwd` : 显示当前的绝对路径
4. `git add <File>` : 把文件加入到仓库中
5. `git commit -m "注释部分"` : 提交添加, 并添加注释
6. `git status` : 显示文件的状态, 如文件变更了, 该命令会显示发生变更的文件.
7. `git diff <File>` : 显示特定文件详细变更位置和内容, 配合`status`找出发生过变化的文件进行使用
8. `git log` : 显示提交的详细记录, 可加`--pretty=oneline`属性方便查看
9. `git reset --hard HEAD^` : 回退到上一个版本， `HEAD^^`为上上个版本， `HEAD~100`为上100个版本, 还可以指定commit id进行回退
10. `git reflog` : 查看历史命令的记录
11. `git checkout -- file` : 返回之前添加或提交时的状态, 也就是回退到暂存区的状态