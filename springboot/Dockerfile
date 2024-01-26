FROM eclipse-temurin:17-jdk-alpine:
    Specifies the base image for the Docker container. In this case, it uses the Eclipse Temurin (formerly AdoptOpenJDK) 17 JDK with the Alpine Linux distribution, known for its small size.

VOLUME /tmp:
    Creates a volume named /tmp. Volumes in Docker are used to share data between the host machine and the container.

COPY target/*.jar app.jar:
    Copies all the JAR files in the target directory (assuming a Maven project structure) from the local build context into the container, and renames it to app.jar.

ENTRYPOINT ["java","-jar","/app.jar"]:
    Specifies the default command to run when the container starts. In this case, it runs the Java command to execute the JAR file (/app.jar), making it the entry point for the container.
    