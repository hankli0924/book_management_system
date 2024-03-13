### 以下是对项目目录结构的介绍
* requirement.txt 记录项目所有的依赖包, 通过pip install -r requirement.txt 来安装
* book_management_system子目录存储整个项目配置信息以及入口文件(url routing)
   * postgres-docker-compose.yml 用于在本地启动项目数据库 ,具体命令如下,详情参考yml文件
     * docker pull postgres 
     * ./postgres_data 是数据库在本地的存储目录
     * docker-compose -f  postgres-docker-compose.yml up -d 
     * docker-compose -f  postgres-docker-compose.yml stop -d 
* books是应用代码，因目前项目中只有一个应用，所以放在顶级目录之下，如后期有更多应用,可以更改目录结构为apps/books
