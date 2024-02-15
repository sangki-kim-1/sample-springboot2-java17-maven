# 샘플 자바11 스프링2 프로젝트

## build
```shell
./mvnw clean install
```

## run
### 1. Internal 통신 - H2 InMemory
```
java -jar target/sample-spring-boot-2-java-maven-0.0.1-SNAPSHOT.jar -spring.profiles.active=internal
```

### 2. External 통신
```
java -jar target/sample-spring-boot-2-java-maven-0.0.1-SNAPSHOT.jar -spring.profiles.active=external
```
