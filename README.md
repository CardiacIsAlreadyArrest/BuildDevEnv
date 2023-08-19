# 用于快速搭建开发环境，可以用vscode在golang容器里进行开发。
mysql，redis数据库的管理工具也配备了，用户名密码在.env文件里。
golang容器开放端口在docker-compose文件中可以看到，一共是11个，1个拿来做api,其他的拿来做rpc。

# 使用说明
用终端打开dousheng-hertz文件夹 运行 docker-compose up
用vscode附加在容器里，在容器里 git clone 项目即可进行开发
