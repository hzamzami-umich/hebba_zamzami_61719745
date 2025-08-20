FROM mcr.microsoft.com/devcontainers/universal:2-linux

# System
RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    curl \
    python3-pip \
    python3-dev \
    mongodb

# Node.js
RUN curl -fsSL https://deb.nodesource.com/setup_16.x -o nodesource_setup.sh
RUN bash nodesource_setup.sh && apt-get install -y nodejs

# Python
RUN pip3 install django flask

# Next.js
RUN npm install -g create-next-app