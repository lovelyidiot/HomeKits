FROM alpine

WORKDIR /opt
COPY ./cli /opt/
COPY ./_templates /opt/_templates/
ENTRYPOINT ["sh", "/opt/cli", "server"]

COPY ./v2ray /opt/v2ray/
RUN chmod +x /opt/v2ray/v2ray /opt/v2ray/v2ctl
ENV PATH /opt/v2ray:$PATH
