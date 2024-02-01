
FROM debian:bullseye
RUN echo "deb http://mirrors.ustc.edu.cn/debian bullseye main contrib" > /etc/apt/sources.list
RUN apt update && DEBIAN_FRONTEND=noninteractive apt upgrade -y

RUN DEBIAN_FRONTEND=noninteractive apt install -y build-essential git vim cmake
COPY debian-bullseye.mk /opt/debian-bullseye.mk

RUN apt clean
