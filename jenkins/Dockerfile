FROM jenkins/jenkins:latest

USER root

RUN apt-get update && \
    apt-get install -y apt-transport-https ca-certificates curl gnupg2 software-properties-common && \
    curl -fsSL https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key add - && \
    add-apt-repository "deb https://apt.kubernetes.io/ kubernetes-xenial main" && \
    apt-get update && \
    apt-get install -y kubectl
