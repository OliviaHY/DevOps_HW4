FROM    alpine:3.2
MAINTAINER  yhuang34@ncsu.edu

RUN apk update && \
    apk add socat && \
    echo 'Hello there!' > task1.txt

EXPOSE 9001  
CMD socat TCP4-LISTEN:9001,reuseaddr,fork SYSTEM:"cat /task1.txt"
