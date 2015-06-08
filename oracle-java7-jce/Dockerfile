FROM pedjak/oracle-java:7
MAINTAINER Predrag Knezevic <pedjak@gmail.com>

RUN cd /tmp && \
	curl -LO "http://download.oracle.com/otn-pub/java/jce/7/UnlimitedJCEPolicyJDK7.zip" -H 'Cookie: oraclelicense=accept-securebackup-cookie' && \
	unzip UnlimitedJCEPolicyJDK7.zip && \
	cp -v UnlimitedJCEPolicy/*.jar /usr/lib/jvm/java-7-oracle/jre/lib/security/ && \
	rm -rf UnlimitedJCEPolicy*
