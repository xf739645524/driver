ifneq ($(KERNELRELEASE),)

obj-m :=drv_buzzer.o

else

KDIR := /home/houstar/GitRepo/driver-ok6410-3.9/linux
all:
	make -C $(KDIR) M=$(PWD) modules
install:
	cp drv_buzzer.ko /srv/nfs/ok6410/lib/modules/3.8.8+
clean:
	make -C $(KDIR) M=$(PWD) clean
endif
