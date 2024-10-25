#前提：GPU驱动已经安装好
1、没有安装nvidia-docker的，先参考下边的链接内容安装
https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html
2、允许本地用户访问当前X服务器
	xhost +local: 
3、获取docker-compose.yml文件到工作目录(act_galaxea_a1)
4、运行星海图机械臂A1环境
	docker-compose up -d
	此处提供两种完成实验的方式
	1）不需要进入容器完成实验

		
	2）需要进入容器，执行下面命令，让后按照实验说明完成实验
		`docker-compose exec sl_proj1`


