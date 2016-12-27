FROM go-php:latest
MAINTAINER "zhoujun" <dev.zhoujun@gmail.com>

RUN yum install -y wget

RUN wget http://repo.mysql.com/mysql-community-release-el7-5.noarch.rpm \
    && rpm -ivh mysql-community-release-el7-5.noarch.rpm \
    && rm -f mysql-community-release-el7-5.noarch.rpm \
    && yum install -y mysql-server \
    && mysql_install_db --user=mysql

RUN yum install -y redis

ENTRYPOINT ["/bin/bash"]
