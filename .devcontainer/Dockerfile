FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt update \
 && DEBIAN_FRONTEND="noninteractive" \
 && apt install -y \
        git \
        clang-format \
        ninja-build \
        gdb \
        bsdmainutils \
        python3 \
        python3-pip \
        python3-dev\
        python3-setuptools \
        strace \
        vim \
        less \ 
        nano \ 
        wget \ 
        curl \
        binwalk \
        file \
        binutils

WORKDIR /home
 #  pwngdb
RUN apt-get update \
    && apt-get install -y \
        git \
        sudo \
    && rm -rf /var/lib/apt/lists/* \
    && python3 -m pip install --upgrade ropper \
    && DSTDIR=/opt \
    && cd ${DSTDIR} \
    && git clone https://github.com/pwndbg/pwndbg \
    && cd pwndbg && ./setup.sh


RUN pip install llvmlite
RUN git clone https://github.com/cea-sec/miasm.git
RUN cd ./miasm* && \
    pip install -r requirements.txt \
    && pip3 install .

RUN pip install frida-tools frida
