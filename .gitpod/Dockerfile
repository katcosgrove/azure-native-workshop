FROM gitpod/workspace-full:latest

RUN curl -fsSL https://get.pulumi.com | sh -s -- --version 3.24.1 && \
    curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash

ENV PATH="${PATH}:/home/gitpod/.pulumi/bin"