# Use the official OpenJDK image as the base image
FROM openjdk:17-jdk-slim

# Set the working directory in the container
WORKDIR /usr/src/jersey

# Copy the compiled class files into the container
COPY . .
run javac Main.java

# Command to run the Java program
CMD ["java", "Main"]
