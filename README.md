```console
% docker network ls
% docker network create redis-network
% docker run -d --rm --network redis-network -p 6379:6379 --name redis-server redis
% docker run -it --rm --network redis-network redis redis-cli -h redis-server ping
PONG
% docker run -d --rm --network redis-network -p 5540:5540 --name redisinsight redis/redisinsight
```

Next, point your browser to [http://localhost:5540](http://localhost:5540)
