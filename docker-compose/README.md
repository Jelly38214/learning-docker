### services之间相互访问
  默认情况下,docker-compose会建立一个默认的网络,名称为docker-compose.yml所在的目录名称(小写)_default.如,example_default
  这个默认的网络会对所有service生效,以便它们能够通过service名称相互访问. 比如有个redis服务和node服务,node服务想要连接上redis, 就可以通过redis:6379这个地址来连接,需要将redis:6379配置到environment,node才能通过process.env.redis_service_addr来获取到
  ```yml
    node:
      environment:
        redis_service_addr: redis:6379
  ```
  Reference:
  * https://zhuanlan.zhihu.com/p/382779160