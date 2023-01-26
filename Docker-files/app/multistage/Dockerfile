FROM openjdk:15.0.2 AS BUILD_IMAGE
RUN yum update && yum install maven -y
RUN git clone https://github.com/muzmmilkhan/quiz_app.git
RUN cd quiz_app && mvn install

FROM openjdk:15.0.2
EXPOSE 8080
COPY --from=BUILD_IMAGE quiz_app/target/SpringBootQuizApp-0.0.1-SNAPSHOT.jar SpringBootQuizApp-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java", "-jar", "/SpringBootQuizApp-0.0.1-SNAPSHOT.jar"]
