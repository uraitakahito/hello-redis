```console
% docker network create redis-network
% docker run -it --rm --network redis-network --name redis-server -d redis
% docker run -it --rm --network redis-network redis redis-cli -h redis-server ping
```
