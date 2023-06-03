FROM alpine

WORKDIR /opt
COPY ./boot.sh ./cli /opt/
COPY ./_templates /opt/_templates/
ENTRYPOINT ["sh", "/opt/cli", "server"]

COPY ./v2ray /opt/v2ray/
ENV PATH /opt/v2ray:$PATH
