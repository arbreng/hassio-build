#FROM arm32v6/alpine:3.7
FROM forumi0721/alpine-armhf-base:latest

RUN ["docker-build-start"]

#COPY qemu-arm-static /usr/bin/qemu-arm-static
RUN apk upgrade --no-cache \
    && apk add --no-cache bash jq tzdata ca-certificates

RUN ["docker-build-end"]

ENTRYPOINT ["/bin/bash", "-c"]
