FROM docker.elastic.co/kibana/kibana-oss:6.6.2
USER root
WORKDIR /usr/share/kibana/

RUN chown kibana:kibana config/kibana.yml

# install open distro security plugin to Kibana
RUN bin/kibana-plugin install https://d3g5vo6xdbdb9a.cloudfront.net/downloads/kibana-plugins/opendistro-security/opendistro_security_kibana_plugin-0.8.0.0.zip

USER kibana

EXPOSE 5601
