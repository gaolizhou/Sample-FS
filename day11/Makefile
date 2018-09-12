#
# Makefile for Linux samplefs
#
CONFIG_MODULE_SIG=n
obj-m += samplefs.o

samplefs-objs := super.o inode.o file.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
