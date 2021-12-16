# Curl request to Spring Initializr

## confirm sample of Initializr
```
curl https://start.spring.io/
```

## create sample package using Initializr
```
curl https://start.spring.io/starter.tgz \
-d name=st_app \
-d packageName=com.st_app \
-d dependencies=web,thymeleaf \
-d type=maven-project | tar -xzvf -
```

## start spring-boot
```
./mvnw spring-boot:run
```

## request
```
curl localhost:8080
```