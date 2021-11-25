FROM centos:centos7

# install tools
RUN yum update -y 
RUN yum install -y sudo vim wget

USER root
COPY ./entrypoint.sh /
RUN chmod 755 /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]

CMD ["/bin/bash"]
