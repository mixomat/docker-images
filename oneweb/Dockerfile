FROM tomcat:8-jre8

ADD com.allianz.oneweb.sdk.*.zip /data/

# extract oneweb sdk
RUN unzip -o /data/com.allianz.oneweb.sdk.*.zip
RUN rm /data/com.allianz.oneweb.sdk.*.zip

# db change management
WORKDIR $CATALINA_HOME/oneweb/data
RUN java -jar com.allianz.oneweb.core.db.change.management.app.jar

EXPOSE 8081

CMD ["catalina.sh", "run"]
