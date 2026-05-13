FROM eclipse-temurin:21-jre-alpine

RUN mkdir -p /app/config /app/data /app/logs && \
    chmod -R 777 /app/config /app/data /app/logs

ENV TZ=Asia/Kolkata
# Set working directory
WORKDIR /app

COPY . .

EXPOSE 2458

CMD ["sh", "-c", "java $JAVA_OPTS -jar dc.jar"]

#tywyuss
