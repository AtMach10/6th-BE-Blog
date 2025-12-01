# 1. 베이스 이미지 지정 (OpenJDK 23)
FROM eclipse-temurin:23-jdk-alpine

# 2. JAR 파일 위치 지정 (Gradle 빌드 결과)
ARG JAR_FILE=build/libs/*.jar

# 3. 컨테이너 내로 복사
COPY ${JAR_FILE} app.jar

# 4. 컨테이너 시작 시 실행
ENTRYPOINT ["java","-jar","/app.jar"]

# 5. 외부 노출 포트
EXPOSE 8080