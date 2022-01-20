FROM openjdk:8-jre-alpine
RUN echo "Asia/Shanghai" > /etc/timezone
ADD canal.adapter-1.1.5.tar.gz /opt/canal/adapter/

WORKDIR /opt/canal/adapter

ENTRYPOINT ["sh", "-c", "sh bin/startup.sh && tail -F logs/adapter/adapter.log"]