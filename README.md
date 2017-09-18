Build this docker image to get access to docker in your CI build

Adapted from here http://container-solutions.com/running-docker-in-jenkins-in-docker/

Run your image with 

```docker run -it -v /var/run/docker.sock:/var/run/docker.sock -v $(which docker):/usr/bin/docker -p 8080:8080 <<your image>>```
