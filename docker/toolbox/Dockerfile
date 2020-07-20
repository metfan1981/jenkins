FROM alpine
RUN apk add --no-cache curl wget busybox-extras netcat-openbsd py-pip bash && \
    pip install awscli
RUN apk --purge -v del py-pip
CMD echo "Dockerfile change commit #1"
