FROM openjdk:8
RUN apt-get update -y
RUN  apt install awscli -y
ENV DATE ${var_name} 
RUN  aws s3 cp s3://frontend-max/GeoIP_$DATE /usr/share/GeoIP --recursive
ADD https://download.newrelic.com/newrelic/java-agent/newrelic-agent/current/newrelic-agent.jar /opt/newrelic.jar
ADD newrelic.yml /opt/newrelic.yml
