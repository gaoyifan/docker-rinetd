```
DOCKER_DIR=/srv/docker/rinetd

docker run -itd --restart=always \
    --name=rinetd \
    --net=host \
    -v $DOCKER_DIR/conf:/etc/rinetd \
    -v $DOCKER_DIR/log:/var/log \
    gaoyifan/rinetd
```
