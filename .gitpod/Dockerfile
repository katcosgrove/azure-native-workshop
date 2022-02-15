FROM gitpod/workspace-full:latest

RUN curl -fsSL https://get.pulumi.com | sh -s -- --version 3.24.1 && \
    sudo -H /usr/bin/pip3 install pulumi && \
    pip3 install pulumi && \
    curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash

RUN sudo apt install python3.8-venv
    
RUN sed -i 's/export PIP_USER=yes/export PIP_USER=no/g' /home/gitpod/.bashrc

ENV PATH="${PATH}:/home/gitpod/.pulumi/bin"
ENV PIP_USER=no
