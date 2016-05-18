#makefile for XR17c15x PCI UARTs for Linux 2.6.31 Kernel  - openSuse 11.2
KERNEL_SRC = /lib/modules/`uname -r`/build

all: build

obj-m += xr17c15x.o

xrpci-objs :=	xr17c15x.o

EXTRA_CFLAGS += -DDEBUG=1

build:
	$(MAKE) -C $(KERNEL_SRC) SUBDIRS=$(PWD) modules

clean:
	rm -f *~ *.o
	rm -f *~ *.ko
