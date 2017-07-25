FROM centos
RUN yum -y install epel-release
RUN rpm -Uvh http://rpms.famillecollet.com/enterprise/remi-release-7.rpm
RUN yum install -y --enablerepo=remi,remi-php70 php php-devel php-mbstring php-mysql php-xml php-mcrypt
RUN systemctl enable httpd

ADD conf/httpd.conf /etc/httpd/conf/httpd.conf

VOLUME application /tmp/app

ENTRYPOINT ["/sbin/init"]
