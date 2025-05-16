# Spring Boot Demo

This assumes you have Docker installed.

## Setup in WSL / Linux

If you want to build things locally (not required for running this repo's build):
```
sudo apt update
sudo apt install openjdk-17-jdk maven -y
```

Then:

```
cd /mnt/c/Users/yourname/Desktop/spring-boot-demo
./mvnw clean package

docker build -t springboot-demo .
docker run -p 8080:8080 springboot-demo
```

Then:

[http://localhost:8080](http://localhost:8080/hello)
