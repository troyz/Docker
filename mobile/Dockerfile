FROM centos:7

RUN curl -sL https://rpm.nodesource.com/setup_6.x | bash -; \
yum install epel-release; \
yum -y install nodejs npm zip; \
yum clean all; \
npm install -g ionic; \
npm install -g cordova-hot-code-push-cli; \
ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime; \
echo "Asia/Shanghai" >> /etc/timezone; \


# docker build -t centos:mobile .
# docker run -it -v /Users/issuser/Desktop/zhangxd/projects/travel/code:/home/code -p 8100:8100 --name ionic centos:mobile bash