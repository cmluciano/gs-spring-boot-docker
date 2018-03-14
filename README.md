﻿# gs-spring-boot-docker
.\mvnw package

java -jar target/gs-spring-boot-docker-0.1.0.jar

docker build  -t registry.ng.bluemix.net/aa_dev01/gs-spring-boot-docker:latest --rm=true .

docker run -p 8080:8080 -d --rm -t registry.ng.bluemix.net/aa_dev01/gs-spring-boot-docker:latest



