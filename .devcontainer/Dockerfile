#FROM ubuntu:latest
FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04
RUN apt-get update && apt-get -y upgrade && apt-get -y install curl texlive texlive-pictures texlive-science latexmk zip unzip build-essential

USER vscode
RUN curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y && \
  /home/vscode/.cargo/bin/cargo install tex-fmt