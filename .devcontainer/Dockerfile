# See here for image contents: https://github.com/microsoft/vscode-dev-containers/tree/v0.154.0/containers/cpp/.devcontainer/base.Dockerfile

ARG VARIANT
FROM mcr.microsoft.com/vscode/devcontainers/cpp:0-${VARIANT}

# Install:gcc-10, g++-10
RUN export DEBIAN_FRONTEND=noninteractive && \
    sudo apt-get update && \
    sudo apt-get -y install software-properties-common && \
    sudo add-apt-repository -y ppa:ubuntu-toolchain-r/ppa && \
    sudo apt update && \
    sudo apt-get -y install g++-10
