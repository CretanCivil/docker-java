FROM tomcat:8.5.15-jre8-alpine
MAINTAINER leapar <leapar@gmail.com>

ADD conf/tomcat/tomcat-users.xml /usr/local/tomcat/conf/tomcat-users.xml
ADD conf/tomcat/context.xml /usr/local/tomcat/webapps/manager/META-INF/context.xml

ADD conf/tomcat/war/app.war /usr/local/tomcat/webapps/app.war
ADD conf/tomcat/war/app-core.war /usr/local/tomcat/webapps/app-core.war



#docker run  -e MYSQL_ROOT_PASSWORD=123456 -e MYSQL_ROOT_HOST=% -p 3306:3306 -d mysql/mysql-server:5.7