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

## Docker Process

### Docker running Process

```
$ docker ps
```

### Docker running and stopping all process

```
$ docker ps -a
```

### Docker stop process

```
$ docker stop <image_id>
```

### Docker stop all process

```
docker stop $(docker ps -qa)
```

### Docker remove all process

```
$ docker rm $(docker ps -qa)
```

## Docker build image

```
$ docker build -t <image_name>:<tag> .
```