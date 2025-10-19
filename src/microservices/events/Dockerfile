FROM eclipse-temurin:21-jre-alpine

WORKDIR /app

COPY events-1.0.jar app.jar

RUN adduser -D appuser && chown appuser:appuser app.jar

USER appuser

EXPOSE 8082

CMD ["java", "--enable-preview", "-jar", "app.jar"]
