FROM apache/kafka:3.7.0

ADD jolokia-agent-jvm-2.0.2-javaagent.jar /opt/kafka/jolokia/jolokia-agent.jar

ENV EXTRA_ARGS='-javaagent:/opt/kafka/jolokia/jolokia-agent.jar=port=7777,host=*'

CMD [ "/etc/kafka/docker/run" ]