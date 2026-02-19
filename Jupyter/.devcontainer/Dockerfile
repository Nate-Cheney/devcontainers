FROM debian:stable

RUN apt-get update && apt-get install -y curl \
    curl \
    git \
    python3 \
    python3-dev \
    python3-pip \
    python3-venv \
    sudo \
    wget \
    unzip

RUN useradd -m -s /bin/bash -G sudo vscode && \
    echo '%sudo ALL=(ALL) NOPASSWD:ALL' >> /etc/sudoers

USER vscode

