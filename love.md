
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
	
	
