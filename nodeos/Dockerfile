FROM ubuntu:bionic
RUN apt-get update && apt-get install --no-install-recommends -y wget  libicu60  libusb-1.0-0 libcurl3-gnutls && rm -rf /var/lib/apt/lists/*
RUN wget --no-check-certificate https://github.com/eosio/eos/releases/download/v1.8.6/eosio_1.8.6-1-ubuntu-18.04_amd64.deb && apt install ./eosio_1.8.6-1-ubuntu-18.04_amd64.deb
ADD . /app
ENTRYPOINT ["/bin/sh", "/app/entrypoint.sh"]
EXPOSE 8888/tcp
EXPOSE 9876/tcp