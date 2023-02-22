FROM mcr.microsoft.com/devcontainers/base:jammy

RUN apt update && \
    apt install -y make build-essential && \
    curl -O https://dl.google.com/go/go1.20.1.linux-amd64.tar.gz && \
    tar zxvf go1.20.1.linux-amd64.tar.gz && \
    mv go /usr/local/

USER vscode

ENV PATH $PATH:/usr/local/go/bin
