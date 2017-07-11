#FROM tomcat:8.5.15-jre8-alpine
#FROM bitnami/tomcat:latest
FROM davidcaste/alpine-tomcat:jdk8tomcat7
MAINTAINER leapar <leapar@gmail.com>

ADD conf/systemInfo.properties /opt/systemInfo.properties
#ADD conf/tomcat/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
#ADD conf/tomcat/context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml

#ADD conf/tomcat/war/apmsys.war /usr/local/tomcat/webapps/apmsys.war
#ADD conf/tomcat/war/app-core.war /usr/local/tomcat/webapps/app-core.war
ADD conf/tomcat/war/apmsys.war /opt/tomcat/webapps/apmsys.war 
#ADD conf/tomcat/server.xml /bitnami/tomcat/conf/server.xml 

#docker run  -e MYSQL_ROOT_PASSWORD=123456 -e MYSQL_ROOT_HOST=% -p 3306:3306 -d mysql/mysql-server:5.7
