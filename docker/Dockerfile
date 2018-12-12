FROM  tomcat:9.0-jre11-slim

COPY server.xml /usr/local/tomcat/conf/
COPY /idplogin.war /usr/local/tomcat/webapps/idplogin.war
COPY /idplogin.xml /usr/local/tomcat/conf/Catalina/localhost/idplogin.xml


#build with:
#maven build

#start on development with:
#docker run --net=cora --volumes-from gatekeeper:ro -p 8082:8080 --name idplogin --link gatekeeper:gatekeeper -d  idplogin


#start on build server with:
#docker run --net=cora-test --volumes-from gatekeeper-test --name idplogin-test --link gatekeeper-test:gatekeeper -d  idplogin

#start on external with:
#docker run --network=cora --name idplogin --link gatekeeper:gatekeeper -d  idplogin
