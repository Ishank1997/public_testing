FROM openjdk:8
ADD aws s3 cp s3://frontend-max/ . --recursive
ADD ./GeoIP /usr/share/GeoIP
ADD https://download.newrelic.com/newrelic/java-agent/newrelic-agent/current/newrelic-agent.jar /opt/newrelic.jar
ADD newrelic.yml /opt/newrelic.yml
