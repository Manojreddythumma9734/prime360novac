FROM eclipse-temurin:21-jre-alpine

RUN mkdir -p /app/data /app/logs /root/myTruststore && \
    chmod -R 777  /app/data /app/logs /root/myTruststore

ENV TZ=Asia/Kolkata

WORKDIR /app

COPY truststore.jks /root/myTruststore
COPY service-registry-3.0.jar /app/service-registry-3.0.jar



CMD ["java", "-jar", "service-registry-3.0.jar"]

