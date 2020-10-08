FROM adoptopenjdk/openjdk11:ubi

COPY kiworkshop-test.jar /test-application/app.jar
WORKDIR /test-application

CMD ["java", "-jar", "-Dspring.profiles.active=prod", "app.jar"]
