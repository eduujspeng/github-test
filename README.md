# github-test
github命令练习

git init 	# 创建命令

git config --global user.name '你自己的github用户名'
git config --global user.email '你自己的github的注册邮箱'

ssh-keygen -t rsa -C "邮箱"    # 创建钥匙
ssh -T git@github.com 		# 验证钥匙

git remote add origin 远程仓库地址		# 关联远程仓库
git remote rm origin				# 删除关联

git pull origin master --allow-unrelated-histories		# 初次拉取远程到本地
git clone 远程地址		# 从远程库克隆到本地

git add '文件名' 				# 添加文件

git commit -m '备注'

git push origin master

git status  

git log 
git log --pretty=oneline   	# 查看版本号与备注
git reflog  	# 查看操作记录

git diff  		# 查看文件的修改内容

git reset --hard HEAD^    # 回到上一个版本
git reset --hard 具体版本号

git checkout --文件名  		# 回到最后一次git commit 或者git add状态

git branch		# 查看分支
git branch 分支名		# 创建分支
git checkout 分支名	# 切换分支
git checkout -b 分支名
git branch -D 分支名 	# 删除分支
git push origin --delete 分支名		#删除远程分支
git merge a分支名		# 把a合并到b分支，先切换到b分支
git log --graph		# 查看分支合并图




example：
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:eduujspeng/Deform_Unet_Plus.git
git push -u origin main

