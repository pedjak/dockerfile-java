FROM pedjak/oracle-java:8
MAINTAINER Predrag Knezevic <pedjak@gmail.com>

RUN cd /tmp && \
	curl -LO "http://download.oracle.com/otn-pub/java/jce/8/jce_policy-8.zip" -H 'Cookie: oraclelicense=accept-securebackup-cookie' && \
	unzip jce_policy-8.zip && \
	cp -v UnlimitedJCEPolicyJDK8/*.jar /usr/lib/jvm/java-8-oracle/jre/lib/security/ && \
	rm -rf UnlimitedJCEPolicy*
