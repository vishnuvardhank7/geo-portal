FROM tomcat:9
MAINTAINER Vishnuvardhan Kesavan

ENV GPTURL=https://github.com/vishnuvardhank7/geoportal/archive/1.0.0.zip

ADD $GPTURL /tmp/geoportal.zip

WORKDIR $CATALINA_HOME/webapps/
RUN unzip /tmp/geoportal.zip *.war
RUN rm /tmp/geoportal.zip

COPY tomcat-users.xml $CATALINA_HOME/conf
