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
    wget https://android.googlesource.com/platform/prebuilts/gcc/linux-x86/aarch64/aarch64-linux-android-4.9/;

