FROM centos:8
MAINTAINER alex4108@live.com
RUN dnf update -y
RUN dnf install -y yum-utils createrepo syslinux genisoimage isomd5sum bzip2 curl file git wget
RUN mkdir ./code && wget -O code/CentOS-8.1.1911-x86_64-boot.iso http://isoredirect.centos.org/centos/8/isos/x86_64/CentOS-8.1.1911-x86_64-boot.iso
CMD ["/bin/bash"]
