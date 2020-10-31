ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
# Example: RUN logstash-plugin install logstash-filter-json

USER root
RUN cd ~ && yum -y update && yum -y install wget && \
        wget https://dev.mysql.com/get/Downloads/Connector-J/mysql-connector-java-8.0.22.tar.gz && \
        tar -xzvf mysql-connector-java-8.0.22.tar.gz && \
        mkdir /mysql-connector && chown -R 1000:1000 /mysql-connector &&\
        mv mysql-connector-java-8.0.22/mysql-connector-java-8.0.22.jar /mysql-connector &&\
        chmod 777 /mysql-connector/mysql-connector-java-8.0.22.jar &&\
        chown -R 1000:1000 /mysql-connector/mysql-connector-java-8.0.22.jar &&\
        rm -rf mysql-connector-java-8.0.22 mysql-connector-java-8.0.22.tar.gz
