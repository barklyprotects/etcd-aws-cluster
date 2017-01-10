FROM alpine:3.4

RUN apk --update add \
      python \
      py-pip \
      jq \
      curl \
      wget \
      bash &&\
    pip install --upgrade awscli &&\
    mkdir /root/.aws

COPY etcd-aws-endpoints /etcd-aws-endpoints

ENTRYPOINT /etcd-aws-endpoints
