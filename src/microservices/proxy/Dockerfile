FROM eclipse-temurin:21-jre-alpine

WORKDIR /app

COPY proxy-1.3.jar app.jar

RUN adduser -D appuser && chown appuser:appuser app.jar

USER appuser

EXPOSE 8000

CMD ["java", "-jar", "app.jar"]
