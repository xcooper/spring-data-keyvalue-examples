Spring Data - Redis Twitter Example
===================================

An improved Java implementation of the [Redis Twitter Clone](https://redis.io/topics/twitter-clone) using Spring Data. Tutorial available [here](https://docs.spring.io/spring-data/data-keyvalue/examples/retwisj/current/)


Build
-----
The project creates a WAR file suitable for deployment in a Servlet 2.5 container (such as Tomcat). It
uses [Gradle](https://gradle.org/) as a build system.
Simply type:

      gradlew build

or if you have gradle installed on your machine and in your classpath:

      gradle build

Start up an instance of the redis server, deploy your WAR and point your browser to (for the typical
setup) [http://localhost:8080/retwisj](http://localhost:8080/retwisj)

Dockerize
---
The project been enhanced with *Docker compose*. Follow the steps to build the environment.

**build the Docker image from the source**
> `gradlew build jibDockerBuild`

**start Docker compose**
> `docker compose up`

**view the page from the HTTP server**
> [main page](http://localhost:8080/retwisj)
