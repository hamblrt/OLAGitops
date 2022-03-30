FROM ibmcom/websphere-liberty:full-java11-openj9-ubi

MAINTAINER a@b.com

RUN mkdir -p /opt/ibm/wlp/usr/shared/apps/SampleWebApp.war

COPY --chown=1001:0 SampleWebApp.war /opt/ibm/wlp/usr/shared/apps/SampleWebApp.war

COPY --chown=1001:0 server.xml /opt/ibm/wlp/usr/servers/defaultServer/
COPY --chown=1001:0 application.xml /opt/ibm/wlp/usr/servers/defaultServer/

ENV LICENSE accept
