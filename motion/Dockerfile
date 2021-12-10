FROM arm32v7/alpine
#ARG BUILD_FROM
#FROM $BUILD_FROM

RUN apk update && apk add -q motion jq

# Copy data
COPY run.sh /
COPY motion.conf /etc/

RUN chmod a+x /run.sh

CMD [ "/run.sh" ]
