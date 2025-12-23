FROM docker.io/texlive/texlive:latest

RUN tlmgr update --self && tlmgr update --all

RUN apt-get update && apt-get install -y tree-sitter-cli && rm -rf /var/lib/apt/lists/*
