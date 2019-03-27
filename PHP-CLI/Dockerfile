# Get latest Ubuntu version
FROM ubuntu:latest

MAINTAINER Temuri Takalandze(ABGEO) <takalandzet@gmail.com>

# Set server timezone
ENV TZ=Asia/Tbilisi
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# Update system
RUN apt-get update

# Install latest PHP version
RUN apt-get install -y php

# Create directory for PHP scripts
RUN mkdir -p /usr/src/scripts

# Set working directory
WORKDIR /usr/src/scripts

# Set volume
VOLUME ["/usr/src/scripts"]

# Run bash
CMD /bin/bash