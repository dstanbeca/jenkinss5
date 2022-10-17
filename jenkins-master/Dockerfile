FROM bitnami/jenkins:latest

USER 0
RUN mkdir /var/log/jenkins
RUN mkdir /var/cache/jenkins
#RUN chown -R jenkins:jenkins /var/log/jenkins
#RUN chown -R jenkins:jenkins /var/cache/jenkins
USER 1001

ENV JAVA_OPTS='-Xmx8192m'
ENV JENKINS_OPTS=' --handlerCountMax=300 -- logfile=/var/log/jenkins/jenkins.log --webroot=/var/cache/jenkins/war'
