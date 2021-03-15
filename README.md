# 마이크로서비스 패턴(길벗, 2020) - Microservices Patterns

- 실습 관련 내용은 '한국어판 부록'을 참고하세요.
- 높은 사양의 PC가 필요합니다(i7계열의 메모리 16GB 이상 권장).

# environment
 - ubuntu 18.04 natural
 - docker install & docker-compose install (recommend for root user.. 😳)
 - after finish install, `sudo usermod -aG docker $USER`
 - set gradle .... (in the book) && ./gradlew assemble (like mvn package, make jar)
 - docker-compose up -d
 - in the cloud system, it is necessary to open port for container /:)
