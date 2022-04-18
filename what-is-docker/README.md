## What is docker containers? (Demo)

#### Install Docker

https://docs.docker.com/get-docker/

#### Docker hello-world to test installed version

```sh
docker run hello-world
```

#### Build Docker image

```sh
docker build -t what_is_docker:latest .
```

#### Run docker container in the background

```sh
docker run -p 5000:5000 -d --name what_is_docker what_is_docker:latest
```

#### Check if container is running

```sh
docker ps
```
or new syntax
```sh
docker container ls 
```

#### Cleanup for all container

```sh
docker stop $(docker ps -aq)
docker rm $(docker ps -aq)
```

#### References

https://www.freecodecamp.org/news/how-to-dockerize-a-flask-app/
