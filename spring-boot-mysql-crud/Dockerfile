FROM openjdk:8-jdk-alpine
ADD target/notes-crud-mysql-springboot.jar notes-crud-mysql-springboot.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "notes-crud-mysql-springboot.jar"]