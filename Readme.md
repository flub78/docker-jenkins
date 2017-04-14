# flub78/jenkins

A jenkins server with some usual tools for static analysis and unit tests

## Build
docker build -t flub78/jenkins .

## Usage
for testing:
docker run --rm -ti -p 18080:8080 -p 15000:50000 -v /data/docker/jenkins:/var/jenkins_home flub78/jenkins /bin/bash

launch the jenkins server:
docker run --rm -p 18080:8080 -p 15000:50000 -v /data/docker/jenkins:/var/jenkins_home flub78/jenkins
