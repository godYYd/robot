1.安装完成git后，在自己电脑上选择工作目录，右键选择Git Bash Here进入
2.如果是第一次进入，则要首先进行登录设置
	在命令行输入
	$ git config --global user.name "你的用户名"
	$ git config --global user.email "你的邮箱"
3.库的连接
	a.创建SSH Key
		$ ssh-keygen -t rsa -C "你的邮箱"
		运行后连按三次回车
	b.查看公钥
		$ cat ~/.ssh/id_rsa.pub
		查看后将公钥复制发给项目创建者并等待创建者添加你的公钥
	c.将当前目录变成git可管理的库
		$ git init
	d.关联项目远程库
		$ git remote add origin git@github.com:godYYd/robot.git
4.从远程库克隆
	$ git clone git@github.com:godYYd/robot.git
5.分支管理教程
	https://www.liaoxuefeng.com/wiki/896043488029600/896954848507552


完成上述步骤并完成教程学习后，在README.md中添加一条能证明自己的信息，如xxx’change（注意不要修改其他文件），如出现冲突，要求按教程合并解决冲突后上传，而不是覆盖。