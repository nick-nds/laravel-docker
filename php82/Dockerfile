FROM webdevops/php-nginx:8.2-alpine

COPY ./sites-available/* /opt/docker/etc/nginx/conf.d/

WORKDIR /app

RUN chown -R application:application /app

USER application
