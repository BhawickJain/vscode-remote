# Get the base Ubuntu image from Docker Hub
FROM ubuntu:latest

# Update apps on the base image
RUN apt-get -y update && apt-get install -y

# Install the Cland compiler
RUN apt-get -y install clang gdb

# Copy the current folder which contains C++ source code to the Docker image under /workspace
COPY  ./workspace /usr/workspace

# Specify the working directory
WORKDIR /usr/workspace

# Use Clang to compile the Test.cpp source file
RUN clang++ -o Test Test.cpp

# Run the output program from the previous step
CMD ["./Test"]
