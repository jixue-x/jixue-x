FROM public-cn-beijing.cr.volces.com/public/nginx:latest

WORKDIR ./douyincloud-nodejs-koa-demo-nginx_static_resource/wwwroot

COPY ./douyincloud-nodejs-koa-demo-nginx_static_resource/run.sh /opt/application/

COPY ./douyincloud-nodejs-koa-demo-nginx_static_resource/nginx.conf /etc/nginx/conf.d/default.conf

RUN chmod -R 777 /opt/application/run.sh

# 拷贝静态资源
COPY ./douyincloud-nodejs-koa-demo-nginx_static_resource/wwwroot .

EXPOSE 8000

CMD /opt/application/run.sh
