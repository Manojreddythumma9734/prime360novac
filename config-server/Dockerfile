FROM eclipse-temurin:21-jre-alpine

RUN mkdir -p /app/config /app/data /app/logs && \
    chmod -R 777 /app/config /app/data /app/logs

ENV TZ=Asia/Kolkata
# Set working directory
WORKDIR /app

COPY config-3.0.jar /app/config-3.0.jar
COPY config/ /app/config

EXPOSE 2458

CMD ["sh", "-c", "java $JAVA_OPTS -jar config-3.0.jar"]

#trfrhewjeedx