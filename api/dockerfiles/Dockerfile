FROM openjdk:17-jdk

WORKDIR /app

ARG JAR_FILE=./build/libs/*.jar

COPY ${JAR_FILE} COTL-1.0.jar

ENV PROFILES prod

EXPOSE 80

ENTRYPOINT ["java", "-Dspring.profiles.active=${PROFILES}","-jar", "/app/COTL-1.0.jar"]