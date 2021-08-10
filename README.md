### Linux basics
  - use Docker as a non-root user
    `sudo usermod -aG docker {user name}`.
    Remember that you will have to log out and back in for this to take effect!

### Docker命令
  - docker run -d --name={name} {image}:启动一个容器并给它指定的名称
  - docker rm $(docker ps -aq): 删除所有Exited状态的容器
  - docker exec -it {container ID} {command}: 在运行中的容器执行指定的命令，执行完毕后并不更改容器的状态

### Docker镜像发布
  1. 先登录:docker login

### 数据卷volume


Reference:
  - [Docker安装和国内镜像配置](https://get.daocloud.io/#install-docker)
  - [Vagrant下载](https://www.vagrantup.com/downloads.html)
  - [volume的覆盖行为](https://segmentfault.com/a/1190000015684472)