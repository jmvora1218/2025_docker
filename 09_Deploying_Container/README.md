# Deploying Containers

This guide covers the basics of deploying containers using Docker.

## Prerequisites

- Docker installed on your system
- Basic knowledge of Docker commands

## 1. Building a Docker Image

```bash
docker build -t my-app:latest .
```

## 2. Running a Container

```bash
docker run -d --name my-running-app -p 8080:80 my-app:latest
```

- `-d`: Run container in detached mode
- `--name`: Assign a name to the container
- `-p`: Map host port to container port

## 3. Listing Running Containers

```bash
docker ps
```

## 4. Stopping a Container

```bash
docker stop my-running-app
```

## 5. Removing a Container

```bash
docker rm my-running-app
```

## Resources

- [Docker Documentation](https://docs.docker.com/get-started/)

#AWS: 
    https://academind.com/tutorials/aws-the-basics
    https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connect-to-linux-instance.html


## Installing Docker on Linux in General
In the last lecture, you saw the AWS-specific command for installing Docker on a Linux machine:

```amazon-linux-extras install docker````

Of course you might not always want to install it on a AWS EC2 instance though - maybe you are using a different provider.

In that case, you can always follow the Linux setup instructions you find on the official Docker page: https://docs.docker.com/engine/install/ (under "Server").