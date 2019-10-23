FROM ubuntu:18.04
LABEL maintainer="Max Boyar <max.boyar.a@gmail.com>"
RUN apt update && apt -y upgrade
ADD https://github.com/meklis/http-snmpwalk-proxy/releases/download/1.0.0/snmpwalk-proxy-linux-amd64 /opt/snmp-proxy
COPY snmp.conf.yml /opt/snmp.conf.yml
RUN chmod +x /opt/snmp-proxy
ENTRYPOINT ["/opt/snmp-proxy", "-c", "/opt/snmp.conf.yml"]
