FROM i386/alpine:3.7

RUN apk upgrade --no-cache \
    && apk add --no-cache bash jq tzdata ca-certificates

RUN echo "#!/bin/bash" >> /usr/bin/docker-build-start
RUN echo "#!/bin/bash" >> /usr/bin/docker-build-end
RUN chmod u+x /usr/bin/docker-build-start
RUN chmod u+x /usr/bin/docker-build-end

ENTRYPOINT ["/bin/bash", "-c"]
