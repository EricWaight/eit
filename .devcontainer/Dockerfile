ARG VARIANT=16
FROM mcr.microsoft.com/vscode/devcontainers/typescript-node:0-${VARIANT}

RUN apt-get update
RUN apt-get install -y \
    lsb-release \
    curl