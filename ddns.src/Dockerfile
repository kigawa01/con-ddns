FROM openjdk
RUN mkdir /src \
    && mkdir /data \
    && curl https://ci.opencollab.dev//job/GeyserMC/job/Geyser/job/master/lastSuccessfulBuild/artifact/bootstrap/standalone/target/Geyser.jar > /src/Geyser.jar
WORKDIR /data
EXPOSE 16132
CMD ["java", "-jar","-Xmx512M","-Xms512M", "/src/Geyser.jar"]