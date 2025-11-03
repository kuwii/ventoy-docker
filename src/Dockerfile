FROM ubuntu:noble

RUN apt-get update \
 && apt-get upgrade -y \
 && apt-get install -y wget xz-utils

RUN wget -P /opt https://github.com/ventoy/Ventoy/releases/download/v1.1.07/ventoy-1.1.07-linux.tar.gz \
 && tar -xzvf /opt/ventoy-1.1.07-linux.tar.gz -C /opt --strip-components=1 \
 && mv /opt/ventoy-1.1.07 /opt/ventoy \
 && rm /opt/ventoy-1.1.07-linux.tar.gz

WORKDIR /opt/ventoy
CMD ./VentoyWeb.sh -P 24680 -H 0.0.0.0
