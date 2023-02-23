FROM mcr.microsoft.com/devcontainers/base:jammy

RUN apt update && \
    apt install -y python3-pip && \
    pip3 install playwright && \
    playwright install-deps
RUN playwright install chromium && \
    cp -r /root/.cache /home/vscode/.cache && \
    chown -R vscode:vscode /home/vscode/.cache

USER vscode
WORKDIR /home/vscode
