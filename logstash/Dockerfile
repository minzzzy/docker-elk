ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

COPY mysql-connector-java-8.0.11.jar mysql-connector-java.jar
# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json
