FROM centos:centos7

RUN yum update -y && yum update -y
RUN yum install -y java-1.8.0-openjdk 
RUN yum install -y wget
RUN mkdir /usr/local/rundeck/
WORKDIR /usr/local/rundeck
#RUN wget -c http://dl.bintray.com/rundeck/rundeck-maven/rundeck-launcher-2.5.3.jar
RUN wget -c https://dl.bintray.com/rundeck/rundeck-maven/rundeck-3.0.20-20190408.war
RUN useradd -g users -m -s /bin/bash admin
RUN chown -R admin:users /usr/local/rundeck

RUN wget https://github.com/rundeck-plugins/rundeck-winrm-plugin/releases/download/v1.3.3/rundeck-winrm-plugin-1.3.3.jar 
#RUN  mv rundeck-winrm-plugin-1.3.3.jar /usr/local/rundeck/libext/
#RUN chown -R admin:users /usr/local/rundeck

USER admin
WORKDIR /usr/local/rundeck
#CMD ["java","-jar","rundeck-launcher-2.5.3.jar"]
CMD ["java","-jar","rundeck-3.0.20-20190408.war"]

