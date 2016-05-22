---
title: Quickstart your SpringBoot with Spring Initializr
date: 2016-05-21T00:51:52+02:00
---

#Introduction

Spring offers a [Spring Initializr](https://start.spring.io/) to bootstrap your application quickly
The most simple way to use it is to do this :

```
curl https://start.spring.io/starter.zip -o demo.zip
```

It will download a `demo.zip` file to your filesystem that you can extract:

```
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100 50954  100 50954    0     0  38634      0  0:00:01  0:00:01 --:--:-- 38660

ls -ltr
total 104
-rw-r--r--  1 ddewaele  staff  50954 May 21 00:54 demo.zip
````

The zip file contains a complete spring boot application.

```
unzip demo.zip 
Archive:  demo.zip
  inflating: mvnw
   creating: .mvn/
   creating: .mvn/wrapper/
   creating: src/
   creating: src/main/
   creating: src/main/java/
   creating: src/main/java/com/
   creating: src/main/java/com/example/
   creating: src/main/resources/
   creating: src/test/
   creating: src/test/java/
   creating: src/test/java/com/
   creating: src/test/java/com/example/
  inflating: .mvn/wrapper/maven-wrapper.jar
  inflating: .mvn/wrapper/maven-wrapper.properties
  inflating: mvnw.cmd
  inflating: pom.xml
  inflating: src/main/java/com/example/DemoApplication.java
  inflating: src/main/resources/application.properties
  inflating: src/test/java/com/example/DemoApplicationTests.java
```

You can customize the cURL command by providing some additional parameters (groupId,artifactId,....)

```
curl https://start.spring.io/starter.tgz -d dependencies=web,actuator -d groupId=com.ecs -d artifactId=hawkbit.client -d language=java -d type=maven-project -d baseDir=hawkbit.client | tar -xzvf -
```


# References

[Spring initializr Github](https://github.com/spring-io/initializr/)
[Spring Starter](https://start.spring.io/)
