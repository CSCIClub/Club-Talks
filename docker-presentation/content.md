% Docker
% Jared Rickert (jaredrickert52@gmail.com)
% Feb 7, 2017

# Why Docker

## Consistent

Always the same environment regardless of the machine it runs on.

## Sandboxed

App doesn't have access to anything to anything on the file system of the host
unless explicit specified

## light weight

- Low CPU/memory overhead
- Fast boot/shutdown

## easy to ship

- runs anywhere were docker is supported
- easy to package

## Modeling Networks

- able to run 100s of containers with ease

# Installation

## Linux

- Most likely in your repository
- Useful to add your user to the *docker* group

```
sudo gpasswd -a $USER docker
```

## Windows

Windows is able to run docker if you have the a PRO version. Otherwise use
docker-machine that uses virtual-box on the back-end.

## Docker-machine

Sets up a working docker environment in a virtual machine

# Basics

## Docker images

Blueprint for running containers

Get them from Docker hub

```
docker pull ubuntu:latest
```

## Docker Containers

A running image

```
docker run --name ubuntutestdrive -ti ubuntu
docker ps -a
```

## Building your own images

Dockerfiles are the blueprint that are use to build an image

## Docker Hub

- Place to store images
- Explore publicly available images
- Automated builds with git
