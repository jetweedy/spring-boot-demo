# Spring Boot Demo

## Setup in WSL / Linux

```
sudo apt update
sudo apt install openjdk-17-jdk maven -y

cd /mnt/c/Users/yourname/Desktop/spring-boot-demo
./mvnw clean package

docker build -t springboot-demo .
docker run -p 8080:8080 springboot-demo
```
