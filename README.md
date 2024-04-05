# 샘플 자바17 스프링2 프로젝트

# 로컬 빌드 & 실행
## build
```shell
./mvnw clean install
```

## run
### 1. Internal 통신 - H2 InMemory
```
java -jar target/sample-spring-boot-2-java17-maven-0.0.1-SNAPSHOT.jar --spring.profiles.active=internal
```

### 2. External 통신 - MariaDB [or MySQL]
```
java -jar target/sample-spring-boot-2-java17-maven-0.0.1-SNAPSHOT.jar --spring.profiles.active=external
```

# 도커 빌드 & 실행
## build
```shell
docker build -t sample-project .
```

## run
```shell
docker run --rm -d -p 8080:8080 --name sample-project sample-project
```