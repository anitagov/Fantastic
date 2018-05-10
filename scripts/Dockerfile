#FROM ubuntu
FROM anitagov/ubuntu-gcc
# Create and set working directory to build
#WORKDIR /build
#ADD . /build
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update && \
    ./scripts/install-tools && \
    rm -rf /var/lib/apt/lists/*
