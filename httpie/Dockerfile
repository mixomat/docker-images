FROM alpine:latest

RUN apk add --no-cache python3 py3-pip && \
    pip3 install --upgrade pip setuptools httpie && \
    rm -r /root/.cache

ENTRYPOINT [ "http" ]
CMD ["--help"]
