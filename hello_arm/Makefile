TOOLCHAIN=/media/disk2/bin/android-19-arm
SYSROOT=${TOOLCHAIN}/sysroot

CC=${TOOLCHAIN}/bin/arm-linux-androideabi-gcc
CPP=${TOOLCHAIN}/bin/arm-linux-androideabi-g++
AS=${TOOLCHAIN}/bin/arm-linux-androideabi-as
STRIP=${TOOLCHAIN}/bin/arm-linux-androideabi-strip
CFLAGS=-O3 -fPIE -pie -g3 --sysroot=${SYSROOT}

all: hello
hello: hello.c
	${CC} ${CFLAGS} -S hello.c
	${CC} ${CFLAGS} -o hello hello.c
