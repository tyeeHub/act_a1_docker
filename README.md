# act_a1_docker

### *前提：GPU驱动已经安装,程序代码已经下载*

1、没有安装nvidia-docker的，先参考下边的链接内容安装  
- [install nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/latest/install-guide.html)

2、允许本地用户访问当前X服务器
```shell
xhost +local: 
```
3、获取docker-compose.yml文件到工作目录(act_galaxea_a1)

4、在act_galaxea_a1目录下运行星海图机械臂A1环境
```shell

# 启动机械臂环境
docker-compose up -d

#bash进入容器
docker-compose exec sl_proj1 bash

#进入act_a1虚拟环境,接着执行作业中python命令，完成实验
conda activate a1

#删除容器(结束与否都不影响实验，只是为省点资源)
docker-compose down
```
#### PS:如果想不进入容器完成实验，可在docker-compose.yml文件中添加对应的command
