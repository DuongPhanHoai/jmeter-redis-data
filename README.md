# jmeter-redis-data
Connection between Redis and jMeter










Bottom note on Installation
- DOCKER: please refer to the docker main page to install
- REDIS: as folloing command (mix from redis docker guide with https://collabnix.com/how-to-setup-and-run-redis-in-a-docker-container/)
  - Ensure docker command:
    - docker -v
  - Create a dedicated Docker network:
    - docker network create -d bridge some-network
  - Run Redis container
    - docker run -d -p 6379:6379 --name myredis --network redisnet redis
  - Enter into Redis-cli (Docker container terminator for easier)
    - redis-cli
    - set a1 100
    - get a1