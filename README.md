apache-tomcat7
==============

An RPM spec file to install Apache Tomcat 7.0.

To Build:

mkdir /opt/build

sudo yum -y install rpmdevtools && rpmdev-setuptree

wget https://raw.github.com/cflynn5/apache-tomcat7/master/tomcat7.spec -O /opt/build/tomcat7.spec

wget https://raw.github.com/cflynn5/apache-tomcat7/master/tomcat7.init -O /opt/build/opt/build

wget https://raw.github.com/cflynn5/apache-tomcat7/master/tomcat7.sysconfig -O /opt/build/tomcat7.sysconfig

wget https://raw.github.com/cflynn5/apache-tomcat7/master/tomcat7.logrotate -O /opt/build/tomcat7.logrotate

wget http://apache.claz.org/tomcat/tomcat-7/v7.0.53/bin/apache-tomcat-7.0.53.tar.gz -O /opt/build/apache-tomcat-7.0.53.tar.gz

rpmbuild -bb /opt/build/tomcat7.spec
