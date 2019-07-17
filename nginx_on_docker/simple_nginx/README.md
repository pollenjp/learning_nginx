

```shell
user@pc%
docker build --tag="simple-nginx" --file=Dockerfile .
user@pc%
docker build --no-cache --tag="simple-nginx" --file=Dockerfile .
```

```
docker run \
    --detach \
    --rm \
    --name=<name> \
    --volume=</contents/path>:/usr/share/nginx/html:ro \
    <image-name>
```

```shell
docker run \
    --rm \
    --name=nginx1 \
    -p=80:80 \
    simple-nginx:latest
```

```:example
docker run \
    --detach \
    --rm \
    --name=nginx1 \
    -p=80:80 \
    --volume=/home/pollenjp/workdir/git/Learning_Nginx/sample_html/pollenjp.github.io:/usr/share/nginx/html:ro \
    simple-nginx:latest
```
