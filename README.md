dockerfiles
=========================

### node_centos6.6

> CentOS 6.6 Dockerfile for centos6.6 image with node v8.9.1 (carbon)

Get Docker version

    # docker version

Grab Centos 6.6 image from Docker Hub

    # docker pull centos:centos6.6

##### build

Copy the sources down and do the build (inside subdirectory)

    # docker build -t <username>/node_carbon:centos6.6 .

##### run

To run (SSH into container):

    # docker run -it <username>/node_carbon:centos6.6 sh

To run (if port 8080 is open on your host):

    # docker run -d -p 8080:8080 <username>/node_carbon:centos6.6

or to assign a random port that maps to port 80 on the container:

    # docker run -d -p 8080 <username>/node_carbon:centos6.6

To the port that the container is listening on:

    # docker ps

##### test

    # curl http://localhost:8080


##### push

        # docker push <username>/node_carbon:centos6.6