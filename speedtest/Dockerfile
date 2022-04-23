FROM debian:buster-slim

RUN apt-get update && apt-get install -y curl

RUN curl -s https://install.speedtest.net/app/cli/install.deb.sh | /bin/bash

RUN apt-get install -y speedtest

CMD [ "speedtest" ]