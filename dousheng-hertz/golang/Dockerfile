FROM golang:1.20

ENV GOPROXY https://goproxy.cn,direct

# 安装必要的软件包和依赖包
RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y --no-install-recommends \
    curl \
    zip \
    unzip \
    git \
    vim 

# 安装 hz
USER root
RUN go install github.com/cloudwego/hertz/cmd/hz@latest

# $GOPATH/bin添加到环境变量中
ENV PATH $GOPATH/bin:$PATH

# 清理垃圾
USER root
RUN apt-get clean && \
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
  rm /var/log/lastlog /var/log/faillog

# 设置工作目录
WORKDIR /usr/src/code

# 克隆项目
CMD ["git","clone","https://github.com/CardiacIsAlreadyArrest/Douyin_Simple_Demo.git"]
# api服务端口
EXPOSE 8080
# rpc服务端口
EXPOSE 8889 
EXPOSE 8890
EXPOSE 8891
EXPOSE 8892
EXPOSE 8893
EXPOSE 8894
EXPOSE 8895
EXPOSE 8896
EXPOSE 8897
EXPOSE 8898
EXPOSE 8899
