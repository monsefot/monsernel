FROM randomdude/gcc-cross-x86_64-elf

RUN echo "deb http://deb.debian.org/debian/ stretch main contrib non-free" > /etc/apt/sources.list
RUN echo "deb http://deb.debian.org/debian/ stretch-updates main contrib non-free" > /etc/apt/sources.list
RUN echo "deb http://security.debian.org/ stretch/updates main contrib non-free" > /etc/apt/sources.list

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y nasm
RUN apt-get install -y xorriso
RUN apt-get install -y grub-pc-bin
RUN apt-get install -y grub-common

VOLUME /root/env
WORKDIR /root/env
