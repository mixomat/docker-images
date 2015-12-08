FROM tomcat:8-jre8

ADD com.allianz.oneweb.sdk.*.zip /data/

# extract oneweb sdk
RUN unzip -o /data/com.allianz.oneweb.sdk.*.zip
RUN rm /data/com.allianz.oneweb.sdk.*.zip

EXPOSE 8081

CMD ["catalina.sh", "run"]
