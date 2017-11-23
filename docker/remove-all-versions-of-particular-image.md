---
description: Remove all versions of particular image
---

# Remove all versions of particular image

Let's say that there is a docker image on your system with different tags.

```
$ docker images anapsix/alpine-java

REPOSITORY            TAG                 IMAGE ID            CREATED             SIZE
anapsix/alpine-java   8_server-jre        acf12230afec        6 months ago        124MB
anapsix/alpine-java   8_jdk               9c7f038a489b        8 months ago        173MB
anapsix/alpine-java   8u121b13_jdk        2d0accb0e2f8        9 months ago        174MB
```

To remove all three images, you can use the following command

```
docker rmi `docker images anapsix/alpine-java | awk '{ print $3; }' | tail -n +2`
```
