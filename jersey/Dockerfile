# Use the official OpenJDK image as the base image
FROM openjdk:17-jdk-slim

# Set the working directory in the container
WORKDIR /usr/src/jersey

# Copy the source files and configuration into the container
COPY ./src /usr/src/jersey/src
COPY .classpath /usr/src/jersey

# Compile the Java source code into a "bin" directory
RUN mkdir bin && javac -d bin src/jersey/*.java src/module-info.java

# Set the working directory to the "bin" directory
WORKDIR /usr/src/jersey/bin

# Command to run the Java program
CMD ["java", "jersey.Main"]
