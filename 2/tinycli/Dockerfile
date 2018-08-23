FROM centos:latest
LABEL maintainer="me@me.com"
LABEL version="0.1"
LABEL description="my first container"

RUN yum update -y && yum install -y curl
ADD message.txt /message.txt
ADD run.sh /run.sh
RUN chmod a+x /run.sh
ENTRYPOINT ["/run.sh"]
CMD ["https://httpbin.org/user-agent"]
