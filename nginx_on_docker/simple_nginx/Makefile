
build :
	-docker image rm simple-nginx:latest
	docker build --no-cache --tag="simple-nginx" --file=Dockerfile .
	docker run \
		--rm \
		--name=nginx1 \
		-p=80:80 \
		simple-nginx:latest