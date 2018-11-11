

```
docker run \
    --detach \
    --name=<name> \
    --volume=</contents/path>:/usr/share/nginx/html:ro \
    <image-name>
```

```:example
docker run \
    --detach \
    --name=simple_nginx \
    --volume=/home/pollenjp/workdir/git/learning_nginx/nginx_on_docker/contents:/usr/share/nginx/html:ro \
    simple_nginx:latest
```
