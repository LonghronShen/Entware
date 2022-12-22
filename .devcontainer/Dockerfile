FROM ubuntu:22.04

ARG SHA

ARG HTTPS_PROXY
ARG HTTP_PROXY
ARG NO_PROXY

RUN apt update && apt install -y build-essential clang flex g++ gawk gcc-multilib gettext \
    git libncurses5-dev libssl-dev python2-minimal python3-distutils python3-pip rsync unzip zlib1g-dev \
    file wget && pip3 install cmake

ENV SHA=${SHA}
ENV FORCE_UNSAFE_CONFIGURE=1