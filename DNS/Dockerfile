FROM ubuntu:bionic

RUN apt-get update \
  && apt-get install -y \
  bind9 \
  bind9utils \
  bind9-doc \
  iputils-ping \
  net-tools \
  dnsutils \
  vim

COPY named.conf.local /etc/bind

COPY db.ifrn.asa.br /etc/bind

ENTRYPOINT service bind9 start 2>/dev/null && /bin/bash -c "while :; do sleep 10; done"