FROM webdevops/php-nginx-dev:8.2-alpine

COPY ./sites-available/* /opt/docker/etc/nginx/conf.d/

COPY ./nginx/ssl/* /opt/docker/etc/nginx/ssl/

# RUN sh -c "echo $uid $gid $user >> touch.txt"

# remove user with id $uid if it exists
# RUN deluser --remove-home --remove-all-files $user || true

# # remove group with id $gid if it exists
# RUN delgroup $user || true

# RUN addgroup -g $gid $user && adduser -D -u $uid -G $user $user

WORKDIR /app

RUN chown -R application:application /app

USER application
