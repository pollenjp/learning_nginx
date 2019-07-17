FROM nginx:1.15
#  nginx version
#    -  https://nginx.org/
COPY nginx.conf /etc/nginx/nginx.conf

RUN chgrp -R root /var/cache/nginx /var/log/nginx && \
    chmod -R 770  /var/cache/nginx /var/log/nginx
