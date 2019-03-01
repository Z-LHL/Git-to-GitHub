## 1.使用 git 前期配置
	>1.设置名称和邮箱
		git config -global user.name '名称'
		git config -global user.email '邮箱email@example.com'
	>2.创建公钥 (输入完一路回车)
		ssh-keygen -t rsa -C '邮箱email@example.com'
	>3.查看公钥 （进入ssh目录下查看是否已生成公钥）
		cd ~/.ssh
	>4.复制公钥
	（进入目录后打开id_rsa.pub文件全部复制，粘贴到github的Settings页面的 》 SSH and GPG keys 》 SSH keys  》 New SSH key 的key栏中）


## 2.克隆 github 项目
	>1.进入github项目页面复制ssh地址
	>2.本机上打开 git bash 控制台
	>3.cd 到要保存的文件目录下
	>4.开始克隆项目到本地
		git clone 地址(如git@github.com:Z-LHL/text.git)

## 3.提交同步到 github 上
	>1.提交新的文件到暂存区，比如添加一个txt文本
		git add .
	>2.从暂存区提交到git管理区
		git commit -m '本次提交的描述文字'
	>3.从git管理区push到远程仓库
		git push origin master
	>4.第一次发布要加点东西
		git push -u origin master

## 4.COMING SOON
