FROM openjdk
RUN mkdir /src \
    && mkdir /data \
    && cd /src \
    && curl -OL https://github.com/kigawa01/ddns-client/releases/download/4.1/ddns-client-4.1.jar
WORKDIR /data
CMD ["java", "-jar","-Xmx64M","-Xms64M", "/src/ddns-client-4.1.jar","--no-jline"]
STOPSIGNAL ["stop"]