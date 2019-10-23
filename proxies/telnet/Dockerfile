FROM ubuntu:18.04
LABEL maintainer="Max Boyar <max.boyar.a@gmail.com>"
RUN apt update && apt -y upgrade
ADD https://github.com/meklis/telnet-proxy/releases/download/1.0.1/telnet-proxy-linux-amd64 /opt/telnet-proxy
COPY telnet-proxy.conf.yml /opt/telnet-proxy.conf.yml
RUN chmod +x /opt/telnet-proxy
ENTRYPOINT ["/opt/telnet-proxy", "-c", "/opt/telnet-proxy.conf.yml"]
