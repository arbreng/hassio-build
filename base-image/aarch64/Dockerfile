#FROM arm64v8/alpin:3.7
FROM forumi0721/alpine-aarch64-base:latest

RUN ["docker-build-start"]

#COPY qemu-aarch64-static /usr/bin/qemu-aarch64-static
RUN apk upgrade --no-cache \
    && apk add --no-cache bash jq tzdata ca-certificates

RUN ["docker-build-end"]

ENTRYPOINT ["/bin/bash", "-c"]
