
				工作目录 -----》  暂存区 -----〉  提交

1. 创建一个文件夹
2. cd到指定文件夹
3. git init（初始化git仓库,生成 .git 隐藏文件夹）
4. git add <文件名>  添加文件到暂存区，让git开始跟踪
5. git commit -m "文件修改备注信息"	提交文件

	git commit -am  "文件修改备注信息"		一次性添加到暂存区并提交

git常见命令：
	git status  查看当前状态
	git reset HEAD <文件名>	将提交的文件恢复暂存区
		git reset HEAD~n	返回上n个快照
	git checkout -- <文件名> 将暂存区文件覆盖当前修改后文件
	git log	参看历史状态
	git diff 	比较暂存区与工作目录
		git diff  快照ID1 快照ID2  	比较历史快照
		git diff  快照ID(HEAD)		比较当前目录和git仓库中的快照
		git diff  --cached [快照ID]		比较暂存区和git仓库中的快照
	git commit --amend		修改提交说明
	git rm <文件名>		删除文件，只是删除工作目录和暂存区文件
	git mv <旧文件名> <新文件名>	修改文件名

git分支：
	git branch "分支名称"		创建分支
	git checkout  分支名称		切换分支

主：终端中绿色文字表示：文件在暂存区等待被提交
		 红色文字表示：文件在工作目录等待被添加到暂存区

