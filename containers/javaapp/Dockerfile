FROM ghcr.io/jhash1/java:1.0.0 AS dev

WORKDIR /app

COPY spring-core-5.0.0.RELEASE.jar /app/spring-core-5.0.0.RELEASE.jar
COPY entrypoint.sh /app/entrypoint.sh
ENTRYPOINT ["sh","entrypoint.sh"]

FROM ghcr.io/jhash1/java:1.0.0 AS prod

WORKDIR /app

COPY spring-core-5.0.0.RELEASE.jar /app/spring-core-5.0.0.RELEASE.jar
COPY entrypoint.sh /app/entrypoint.sh
ENTRYPOINT ["sh","entrypoint.sh"]