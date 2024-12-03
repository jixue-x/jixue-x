来自 public-cn-beijing.cr.volces.com/public/nginx:latest

WORKDIR工作目录 /wwwroot

COPY复制 run.sh /opt/application/

COPY复制 nginx.conf /etc/nginx/conf.d/default.conf

RUN运行 chmod -R 777 /opt/application/run.sh

# 复制静态资源
COPY复制 wwwroot 。

EXPOSE曝光80008000

CMDCMD /opt/application/run.sh
