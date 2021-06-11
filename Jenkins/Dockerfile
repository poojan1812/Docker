FROM centos
RUN yum install wget -y
RUN wget -o /etc/yum.repos.d/jenkins.repo https://pkg.jenkins.io/redhat-stable/jenkins.repo
RUN rpm --import https://pkg.jenkins.io/redhat/jenkins.io.key
RUN yum install net-tools sudo jenkins java-11-openjdk.x86_64 initscripts -y
RUN echo "jenkins ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers
RUN echo "/etc/rc.d/init.d/jenkins start" >> /etc/bashrc
