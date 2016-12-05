# git学习
## 基本操作
- `git init` : 将当前目录作为仓库
- `git config --global user.name "name"`
   `git config --global user.email "email"`
	配置姓名和邮箱, `--global`代表配置所有的, 也可以只分别配置每个不同的 
- `pwd` : 显示当前的绝对路径
- `git add <File>` : 把文件加入到仓库中
- `git commit -m "注释部分"` : 提交添加, 并添加注释
- `git status` : 显示文件的状态, 如文件变更了, 该命令会显示发生变更的文件.
- `git diff <File>` : 显示特定文件详细变更位置和内容, 配合`status`找出发生过变化的文件进行使用
- `git log` : 显示提交的详细记录, 可加`--pretty=oneline`属性方便查看
- `git reset --hard HEAD^` : 回退到上一个版本， `HEAD^^`为上上个版本， `HEAD~100`为上100个版本, 还可以指定commit id进行回退
- `git reflog` : 查看历史命令的记录

## 运程管理
- `git remove add origin url` : 将本地仓库与远程仓库建立连接. 配合push使用
- `git clone url` : 克隆远程仓库到本地仓库(建立连接)
- `git push [-u] origin master` : 将本地仓库的内容push到远程仓库, 一般第一push时带上参数`-u`