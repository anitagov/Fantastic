#Dockerfile to build ubuntu-tools:1.2
FROM anitagov/ubuntu-tools:1.1
# Create and set working directory to build
#WORKDIR /build
#ADD . /build
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get -y update && \
    apt-get -y install sudo && \
    apt-get -y install linux-generic && \
    apt-get -y install kmod && \
    rm -rf /var/lib/apt/lists/*
