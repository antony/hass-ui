ARG BUILD_FROM
FROM $BUILD_FROM

ENV LANG C.UTF-8

COPY run.sh /
RUN apk add --no-cache nodejs
RUN npm install -g sirv-cli
RUN chmod a+x /run.sh

CMD [ "sirv", "start", "public", "-p", "80", "-s" ]