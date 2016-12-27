FROM centos:7
MAINTAINER "zhoujun" <dev.zhoujun@gmail.com>

RUN yum install -y vim git make

RUN yum install -y golang
ENV GOROOT /usr/lib/golang
ENV PATH $GOPATH/bin:PATH

RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm \
    && rpm -Uvh https://mirror.webtatic.com/yum/el7/webtatic-release.rpm \
    && yum install -y php70w-zts php70w-devel php70w-embedded
RUN yum install -y php70w-mcrypt

WORKDIR /data
ENV GOPATH /data
CMD ["/bin/bash"]
