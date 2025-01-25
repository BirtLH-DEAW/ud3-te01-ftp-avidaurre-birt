FROM ubuntu:latest

RUN apt-get update \
&& apt-get install -y nano \
&& apt-get install -y proftpd 

COPY Recursos/proftpd.conf /etc/proftpd/
COPY Recursos /srv/ftp

EXPOSE 21