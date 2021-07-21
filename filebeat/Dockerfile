ARG FILEBEAT_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/beats/filebeat:${FILEBEAT_VERSION}

RUN filebeat modules enable okta

ENTRYPOINT filebeat setup && filebeat -e