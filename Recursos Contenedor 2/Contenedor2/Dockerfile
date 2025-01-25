FROM ubuntu:latest

RUN apt-get update \
&& apt-get install -y nano \
&& apt-get install -y proftpd \
&& apt-get install openssl \
&& mkdir /srv/deaw \
&& useradd deaw -d /srv/deaw -s/sbin/nologin

COPY Recursos /srv/deaw
COPY Recursos/proftpd.conf /etc/proftpd
COPY Recursos/tls.conf /etc/proftpd
COPY Recursos/tlsavidaurre.crt /etc/ssl/certs
COPY Recursos/tlsavidaurre.key /etc/ssl/private

EXPOSE 21