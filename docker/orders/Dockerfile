FROM weaveworksdemos/msd-java:jre-latest

WORKDIR /usr/src/app
COPY *.jar ./app.jar

RUN wget -O dd-java-agent.jar 'https://dtdg.co/latest-java-tracer'

RUN	chown -R ${SERVICE_USER}:${SERVICE_GROUP} ./app.jar

USER ${SERVICE_USER}

ENTRYPOINT ["/usr/local/bin/java.sh","-javaagent:./dd-java-agent.jar","-jar","./app.jar", "--port=80"]
