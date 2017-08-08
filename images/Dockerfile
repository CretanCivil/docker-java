#FROM tomcat:8.5.15-jre8-alpine
#FROM bitnami/tomcat:latest
FROM davidcaste/alpine-tomcat:jdk8tomcat7
MAINTAINER leapar <leapar@gmail.com>

RUN echo "Asia/shanghai" > /etc/timezone
ADD conf/systemInfo.properties /opt/systemInfo.properties
ADD conf/opentsdb.properties /opt/opentsdb.properties

#ADD conf/tomcat/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
#ADD conf/tomcat/context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml

#ADD conf/tomcat/war/apmsys.war /usr/local/tomcat/webapps/apmsys.war
#ADD conf/tomcat/war/app-core.war /usr/local/tomcat/webapps/app-core.war
ADD conf/tomcat/war/apmsys.war /opt/tomcat/webapps/apmsys.war
ADD conf/tomcat/war/alarm-service.war /opt/tomcat/webapps/alarm-service.war
 
ADD tomcat/server.xml /opt/tomcat/conf/server.xml
ADD tomcat/logging.properties /opt/tomcat/conf/logging.properties

CMD ["/opt/tomcat/bin/catalina.sh","run"]
