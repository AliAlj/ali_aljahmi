# Use the default Linux Universal base image
FROM mcr.microsoft.com/vscode/devcontainers/base:ubuntu-22.04

# Install system dependencies
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    npm \
    && apt-get clean && rm -rf /var/lib/apt/lists/*

# Install Flask
RUN pip3 install flask

# Install Vue.js CLI globally
RUN npm install -g @vue/cli

# Set the working directory inside the container
WORKDIR /workspace
