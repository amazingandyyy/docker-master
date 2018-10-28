# Docker master

## docker

```terminal
docker ps
docker ps -a
docker run + <name>
docker run -d <name> (background)
// run = create + start
docker create
docker start + <id>
docker start -a <id> (attach, print into the console)
docker system prune
docker logs <id>
docker stop <id>
docker kill <id>

docker exec -it <id> command (provide input to, in text)
docker exect -i -t
  -i: make my input to stdin
  -t: make sure all text in stdout is beautiful
docker exec -it <id> sh (run the same one)
docker run -it <name> sh
docker build .
docker build -t andy/redis:latest . (tag)
docker commit -c 'CMD ["redis-server"]'
docker run -p 5000:8080 <id> (port mapping, outside:inside)
```

## docker-compose

```terminal
docker-compose up = docker run myimage
docker-compose up -d (background)
docker-compose up --build = docker build . + docker run myimage
<!-- restart policies -->
"no", always, on-failure, unless-stopped

docker-compose ps
```

## docker workflow

```terminal
docker build -f Dockerfile.dev .
```

## Resources

[docker-and-kubernetes-the-complete-guide](https://www.udemy.com/docker-and-kubernetes-the-complete-guide)

## License
[MIT](https://github.com/amazingandyyy/docker-master/blob/master/license)