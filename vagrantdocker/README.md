Linked Data Registry Vagrant Docker Installation
================================================


Sets up and runs the linked data registry on a host machine (running Ubuntu) using Vagrant and Docker. Vagrant builds a docker image from the Dockerfile. Vagrant provisions a docker container created from this image and starts tomcat. Port 8080 is mapped to port 80 on the host machine in the Vagrantfile. 

## Prerequistes

- Ubuntu >14.04 64bit
- Docker >1.0 
- Vagrant >1.6.3

## Instructions

run

```
sudo vagrant up --provider=docker
```

or

```
sudo ./vagrantup.sh
```

for extra debug info run

```
VAGRANT_LOG=debug sudo vagrant up --provider=docker
```