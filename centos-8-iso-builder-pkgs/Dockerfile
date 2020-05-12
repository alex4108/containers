# Preps the Cent8 Container
FROM centos:8
MAINTAINER alex4108@live.com
RUN dnf update -y
RUN dnf install -y yum-utils createrepo syslinux genisoimage isomd5sum bzip2 curl file git wget unzip
RUN mkdir /root/code
RUN curl -L -o /root/code/CentOS-8.1.1911-x86_64-boot.iso http://isoredirect.centos.org/centos/8/isos/x86_64/CentOS-8.1.1911-x86_64-boot.iso
RUN curl -L -o /root/code/bootstrap.zip https://github.com/alex4108/centos-8-minimal/archive/master.zip
RUN unzip /root/code/bootstrap.zip -d /root/code/
RUN mv /root/code/centos-8-minimal-master/* /root/code/
CMD ["/bin/bash"]
