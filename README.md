# docker-springboot-mysql

docker pull mysql

Use MySQL Image published by Docker Hub (https://hub.docker.com/_/mysql/) 
Command to run the mysql container 
 
docker run -p 3306:3306 --name mysql-srikanth-db -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=mydb -e MYSQL_USER=root -e MYSQL_PASSWORD=root -d mysql:latest

docker restart mysql-srikanth-db

cd C:\SRIKANT\workspace2\spring-boot-mysql-crud

docker build . -t notes-crud-mysql-springboot

docker run -p 8080:8080 --name notes-crud-mysql-springboot --link mysql-srikanth-db:mysql -d notes-crud-mysql-springboot

docker restart notes-crud-mysql-springboot

docker logs mysql-srikanth-db

docker logs notes-crud-mysql-springboot

https://stackoverflow.com/questions/51527683/java-net-unknownhostexception-dockerized-mysql-from-spring-boot-application