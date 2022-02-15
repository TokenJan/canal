FROM openjdk:8-jre-alpine

RUN echo "Asia/Shanghai" > /etc/timezone

ADD canal-server.tar.gz /opt

WORKDIR /opt/canal-server

EXPOSE 11110 11111 11112 9100

CMD ["sh", "-c", "sh /opt/canal-server/bin/startup.sh && tail -F /opt/canal-server/logs/rwf/rwf.log"]
