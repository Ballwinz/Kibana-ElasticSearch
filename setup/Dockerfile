FROM docker.elastic.co/elasticsearch/elasticsearch:8.0.0

ARG ELK_VERSION

# https://www.docker.elastic.co/
#FROM docker.elastic.co/elasticsearch/elasticsearch:8.0.0

USER root
RUN mkdir /state && chown elasticsearch /state
USER elasticsearch:root

COPY . /
ENTRYPOINT ["/entrypoint.sh"]
