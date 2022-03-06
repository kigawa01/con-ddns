FROM openjdk
RUN mkdir /src \
    && mkdir /data \
    && curl https://github.com/kigawa01/ddns-client/releases/download/4.1/ddns-client-4.1.jar > /src/ddns-client.jar
WORKDIR /data
EXPOSE 16132
CMD ["java", "-jar","-Xmx64M","-Xms64M", "/src/ddns-client.jar"]