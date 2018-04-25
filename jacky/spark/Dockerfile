FROM debian:latest
RUN apt-get update \
    && apt-get install -y \
        default-jdk scala wget
RUN mkdir /opt/jars

COPY spark /opt/spark
COPY jarSpark.jar /opt/jars

RUN export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-amd64

# On expose les ports
EXPOSE 22
EXPOSE 80
EXPOSE 7077
EXPOSE 9092
EXPOSE 2181
