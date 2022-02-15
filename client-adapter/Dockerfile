FROM openjdk:8-jre-alpine

RUN echo "Asia/Shanghai" > /etc/timezone

ADD canal-adapter.tar.gz /opt

WORKDIR /opt/canal-adapter

EXPOSE 8081

CMD ["sh", "-c", "sh /opt/canal-adapter/bin/startup.sh && tail -F /opt/canal-adapter/logs/adapter/adapter.log"]
