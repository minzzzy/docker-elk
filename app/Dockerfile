FROM adoptopenjdk/openjdk11:ubi

COPY app.jar /test-application/app.jar
WORKDIR /test-application

CMD ["java", "-jar", "-Dspring.profiles.active=prod", "app.jar"]
