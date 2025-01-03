FROM alpine:latest

WORKDIR /usr/local/bin

COPY op-node/bin/op-node /usr/local/bin/op-node

RUN chmod +x /usr/local/bin/op-node

CMD ["op-node", "--help"]
