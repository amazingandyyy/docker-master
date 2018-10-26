# Docker master

commands
```terminal
docker ps
docker ps -a
docker run + <name>
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