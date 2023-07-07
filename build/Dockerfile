FROM alpine:latest

RUN apk update && \
   apk add tor && \
   rm -rf /var/cache/apk/* && \
   echo "Log notice stdout" >> /etc/torrc && \
   echo "SocksPort 0.0.0.0:9150" >> /etc/torrc

EXPOSE 9150

CMD tor -f /etc/torrc
