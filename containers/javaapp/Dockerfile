FROM ghcr.io/jhash1/java:base-dev-b2019ddb1b072da175345ae0ea15f1f8d63d0d3b AS dev

WORKDIR /app

COPY spring-core-5.0.0.RELEASE.jar /app/spring-core-5.0.0.RELEASE.jar
COPY entrypoint.sh /app/entrypoint.sh
ENTRYPOINT ["sh","entrypoint.sh"]

FROM eclipse-temurin:17-jdk-jammy AS prod

WORKDIR /app

COPY spring-core-5.0.0.RELEASE.jar /app/spring-core-5.0.0.RELEASE.jar
COPY entrypoint.sh /app/entrypoint.sh
ENTRYPOINT ["sh","entrypoint.sh"]