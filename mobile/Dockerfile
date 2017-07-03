FROM centos:7

RUN curl -sL https://rpm.nodesource.com/setup_6.x | bash -; \
yum install epel-release; \
yum -y install nodejs npm git zip; \
yum clean all; \
npm install -g ionic; \
npm install -g cordova-hot-code-push-cli; \
npm install -g gulp; \
ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
echo "Asia/Shanghai" >> /etc/timezone; \


## create image
# docker build -t centos:mobile .

## run container on osx
# docker run -it -v /Users/issuser/code:/home/code -p 8100:8100 -p 10001:10001 -p 3001:3001 --name ionic centos:mobile bash

## run container on windows (Please make sure you have assign r+w to `/c/Users/code` for everyone)
# docker run -it -v /c/Users/code:/home/code -p 8100:8100 -p 10001:10001 -p 3001:3001 --name ionic centos:mobile bash
