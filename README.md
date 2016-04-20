# scitools-hacks

export PATH=/opt/scitools/bin/linux64/buildspy:$PATH

export SCITOOL_CROSS_COMPILE=arm-linux-gnueabi-

buildspy -db ~/understand/kernel.udb -cc arm-linux-gnueabi-gcc -cxx arm-linux-gnueabi-cpp -cmd "make ARCH=arm CROSS_COMPILE=sci-linux- -j9 all V=1"
