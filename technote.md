
# why there is no file in the desktop

	sudo apt-get remove tig
	
# 命令行
## 配置git

	git config --global user.name "username"
	git config --global user.email "email"
	
	git config --list


## 生成 ssh key 密钥

	cd ~/.ssh
	ls
	#若不存在密钥
	ssh-keygen -t rsa -C "youremail@example.com"
	#可以看到已经生成好了两个密钥，id_rsa 文件是私钥，不需要上传，id_rsa.pub 文件是公钥，是需要上传的
	#打开github的 setting -> SSH keys，点击右上角 New SSH key，把生成好的公钥 id_rsa.pub 放进 key 输入框中，再为当前的 key 起一个 title 即可

## 下载仓库

	git clone `地址`
	
	git add.
	git ci
	git commit -m "message"
	git commit --help
	git push 
	git push origin <远程分支名>
	
## 本地上传

	#初始化本地仓库
	git init 
	git add README.md 
	git commit -m "first commit"
	git remote add Ceres your_first_git_address
	git push -u Ceres master
	git remote add Mars your_second_git_address
	#需要上传的分支名称为master
	git push -u Mars master
	#显示远端的相关分支
	git show-ref
	#git push --set-upstream的简写形式为git push -u
	#（--set-upstream选项会指定一个默认主机），同时指定该主机为默认主机，后面使用可以不加任何参数使用git push
	git push --set-upstream origin D**

## 本地开发

	#进入文件夹后初始化本地仓库
	git init 
	#upstream一般为他人远端仓库名字，后面接远端仓库地址
	git remote add upstream https://github.com/ant-design/ant-design.git
	#获取远端仓库的master分支最新代码
	git pull upstream master
	#创建分支bugfix
	git checkout -b bugfix
	#切换分支
	git checkout master
	git pull upstream master
	git checkout bugfix
	#把 master 分支的最新 commit 合并到 bugfix 分支
	git rebase master
	把现在的代码 push 到远端的 bugfix 分支,origin一般为自己远端仓库名字
	git push origin bugfix

# 使用技巧
## 快捷键总览 
```shift + ? ```
## 快速查看文件 
```t ```
## 高亮代码
给别人标出重点代码，只需要在发给别人的 GitHub 链接后面加上 ```#L``` 和行号，多行代码用```-```连接


	
	
