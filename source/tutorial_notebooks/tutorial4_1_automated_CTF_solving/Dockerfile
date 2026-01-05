FROM ubuntu:22.04

# 1. System Setup & Basic Tools
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update && apt-get install -y \
    curl wget netcat \
    build-essential gdb gdbserver \
    python3-dev python3-pip python3-venv \
    libssl-dev libffi-dev \
    git bsdmainutils file \
    iputils-ping \
    && rm -rf /var/lib/apt/lists/*

# 2. Install Radare2 (Reverse Engineering Framework)
WORKDIR /tmp
RUN curl -LO [https://github.com/radareorg/radare2/releases/download/5.8.8/radare2_5.8.8_amd64.deb](https://github.com/radareorg/radare2/releases/download/5.8.8/radare2_5.8.8_amd64.deb) && \
    dpkg -i radare2_5.8.8_amd64.deb && \
    rm radare2_5.8.8_amd64.deb

# 3. Install Python CTF & Agent Dependencies
# We install 'pwntools' for exploits and 'langchain' libraries for the Agent logic.
RUN pip3 install --no-cache-dir --upgrade pip && \
    pip3 install --no-cache-dir \
    pwntools \
    angr \
    requests \
    beautifulsoup4 \
    langchain \
    langchain-ollama \
    langgraph \
    docker

# 4. Setup Non-Root User
ARG USERNAME=ctfplayer
RUN useradd -m -s /bin/bash $USERNAME
USER $USERNAME
WORKDIR /home/$USERNAME
RUN mkdir ctf_files

# 5. Entrypoint
CMD ["tail", "-f", "/dev/null"]