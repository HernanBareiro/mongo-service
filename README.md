# Build and start MongoDB container
```shell
docker compose up -d
```
# Test connection with docker
```shell
docker exec -it mongo-service mongo --host localhost --port 27017 -u admin -p admin123 --authenticationDatabase admin
```
# Test conection with mongo client
```shell
mongo mongodb://admin:admin123@localhost:27017
```
# Verify if MongoDB is running
```shell
docker ps | grep mongo
```
# View MongoDB logs
```shell
docker logs mongo-service
```
# Stop container
```shell
docker compose down
```
# Restart container
```shell
docker compose restart
```
# Remove container
```shell
docker compose rm -f
```
# Rebuild container
```shell
docker compose build
```

For more information, please refer to the [MongoDB documentation](https://docs.mongodb.com/manual/installation/) and the [Docker documentation](https://docs.docker.com/engine/reference/commandline/cli/).