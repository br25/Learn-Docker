1. Stop and Remove Containers:
docker rm -f $(docker ps -aq)
2. Remove Images:
docker rmi -f $(docker images -aq)
3. Remove Volumes:
docker volume rm $(docker volume ls -q)
4. Remove Networks:
docker network rm $(docker network ls -q)
5. Remove Dockerfile and Project Directory:
rm -rf /path/to/your/project
6. Remove Unused Data:
docker image prune -f
docker container prune -f
7. Cleanup Everything:
docker system prune -af
