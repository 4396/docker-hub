FROM centos:latest
MAINTAINER "zhoujun" <dev.zhoujun@gmail.com>

RUN yum install -y vim git

RUN yum install -y golang
ENV GOROOT /usr/lib/golang
ENV PATH $GOPATH/bin:PATH
ENV GOPATH /data

RUN rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm \
    && rpm -Uvh https://mirror.webtatic.com/yum/el7/webtatic-release.rpm \
    && yum install -y php70w php70w-devel php70w-embedded

WORKDIR /data

CMD ["/bin/bash"]
