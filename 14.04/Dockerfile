FROM ubuntu:14.04
RUN dpkg --add-architecture i386; \
    apt-get update; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y xz-utils; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y wget; \
    DEBIAN_FRONTEND=noninteractive apt install -y zlib1g; \
    DEBIAN_FRONTEND=noninteractive apt install -y zlib1g-dev; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y device-tree-compiler; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y make; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y git; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y lib32bz2-1.0 lib32z1 lib32ncurses5 lib32ncursesw5 lib32stdc++6 libexpat1-dev:i386; \
    DEBIAN_FRONTEND=noninteractive apt-get install -y scons; \
    cd /home; \
    wget https://armkeil.blob.core.windows.net/developer/Files/downloads/gnu-a/10.2-2020.11/binrel/gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu.tar.xz; \
    tar xf gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu.tar.xz -C /opt/; \
    rm gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu.tar.xz;

ENV PATH="/opt/gcc-arm-10.2-2020.11-x86_64-aarch64-none-linux-gnu/bin:${PATH}"

