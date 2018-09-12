#
# Makefile for Linux samplefs
#
obj-m += samplefs.o

samplefs-objs := super.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) clean
