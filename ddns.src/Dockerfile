FROM openjdk
RUN mkdir /src \
    && mkdir /data \
    && curl -OL -o /src/ddns-client-4.1.jar https://github.com/kigawa01/ddns-client/releases/download/4.1/ddns-client-4.1.jar
WORKDIR /data
CMD ["java", "-jar","-Xmx64M","-Xms64M", "/src/ddns-client-4.1.jar"]