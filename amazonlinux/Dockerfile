FROM stechstudio/aws-lambda-build:1.2.2
LABEL authors="Bubba Hines <bubba@stechstudio.com>"

RUN yum clean all
RUN yum makecache fast && yum install -y libxml2 --nogpgcheck

# Install devel where we can
RUN mkdir -p /deps
RUN mkdir -p /target
RUN mkdir -p /target/modules

# Compiler settings
ENV FLAGS="-O3"