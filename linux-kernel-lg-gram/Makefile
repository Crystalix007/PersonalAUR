obj-m = lg-laptop.o

VER ?= $(shell uname -r)

all:
	make -C ${PREFIX}/lib/modules/${VER}/build M=$(PWD) modules

clean:
	rm -f *.o *.mod.c *.ko modules.order Module.symvers .*.cmd .*.mk .tmp_versions/*.mod
	rm -rf .tmp_versions

install: lg-laptop.ko
	mkdir -p ${DESTDIR}${PREFIX}/lib/modules/${VER}/extra/drivers/platform/x86/
	cp lg-laptop.ko ${DESTDIR}${PREFIX}/lib/modules/${VER}/extra/drivers/platform/x86/
