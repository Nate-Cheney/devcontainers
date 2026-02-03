FROM debian:stable

RUN apt-get update && apt-get install -y \ 
    curl \
    git \
    python3 \
    python3-dev \
    python3-pip \
    python3-venv \
    sudo \
    wget \
    unzip

# Create vscode user with homefolder and add to groups
RUN useradd -m -s /bin/bash -G sudo vscode
# Passwordless sudo
RUN echo '%sudo ALL=(ALL) NOPASSWD:ALL' >> /etc/sudoers
# Set default user
USER vscode
