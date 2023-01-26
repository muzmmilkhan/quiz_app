FROM openjdk:15.0.2
EXPOSE 8080
RUN curl -v -u admin:admin123 -o SpringBootQuizApp-0.0.1-SNAPSHOT.jar http://18.119.109.156:8081/repository/vprofile-release/QA/vproapp/5-23-01-26_19:56/vproapp-5-23-01-26_19:56.jar
ENTRYPOINT ["java", "-jar", "/SpringBootQuizApp-0.0.1-SNAPSHOT.jar"]