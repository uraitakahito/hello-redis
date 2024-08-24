```console
% docker network create redis-network
% docker run -d --rm --network redis-network --name redis-server redis
% docker run -it --rm --network redis-network redis redis-cli -h redis-server ping
% docker run -d --rm --network redis-network --name redisinsight -p 5540:5540 redis/redisinsight
```

Next, point your browser to [http://localhost:5540](http://localhost:5540)
