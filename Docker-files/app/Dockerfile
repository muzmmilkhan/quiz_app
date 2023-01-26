FROM openjdk:15.0.2
EXPOSE 8080
ADD /var/lib/jenkins/workspace/quiz_cicd_pipeline/target/SpringBootQuizApp-0.0.1-SNAPSHOT.jar SpringBootQuizApp-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java", "-jar", "/SpringBootQuizApp-0.0.1-SNAPSHOT.jar"]