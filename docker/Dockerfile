FROM openjdk:21-slim
COPY docker/ /app
WORKDIR /app
RUN ./mvnw package
EXPOSE 8080 
CMD ["java", "-jar", "target/spring-petclinic-3.0.0-SNAPSHOT.jar"] 