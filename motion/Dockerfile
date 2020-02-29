
FROM arm64v8/debian
#ARG BUILD_FROM
#FROM $BUILD_FROM

RUN apt-get update && apt-get install -q -y --no-install-recommends \
    motion \
    jq

# Copy data
COPY run.sh /
COPY motion.conf /etc/

RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
