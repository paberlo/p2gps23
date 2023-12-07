FROM tomcat:7-jre8

COPY drop/mrp.war /usr/local/tomcat/webapps/
COPY drop/index.jsp /usr/local/tomcat/webapps/ROOT/index.jsp

EXPOSE 8080

ENTRYPOINT ["catalina.sh", "run"]

#EXPOSE 8082
#ENTRYPOINT P=8082 ;sed "s/8080/$P/g" < conf/server.xml > /tmp/srv.xml && catalina.sh run -config /tmp/srv.xml