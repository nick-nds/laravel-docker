FROM webdevops/php-nginx-dev:8.2-alpine

COPY ./sites-available/* /opt/docker/etc/nginx/conf.d/

# RUN addgroup -g $gid $user && adduser -D -u $uid -G $user $user

WORKDIR /app

RUN chown -R application:application /app

USER application
