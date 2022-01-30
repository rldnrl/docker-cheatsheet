# docker-cheatsheet

## Docker Image List

```
$ docker image ls
```

```
$ docker images
```

## Docker Run
### Basic Run

```
$ docker run <image_name>:<tag>
```

### Detach Mode

```
$ docker run -d <image_name>:<tag>
```

### Run with Port binding

```
$ docker run -p <host_port>:<container_port> <image_name>:<tag>
```

### Run with Environment

```
$ docker run -e <key>=<value> <image_name>:<tag>
```