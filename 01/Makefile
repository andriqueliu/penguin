ALTPATH = $(altPath)
ifeq ($(ALTPATH),)
	FINALPATH = $(shell uname -r)
else
	FINALPATH = ALTPATH
endif

obj-m += hello.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(PWD) modules
