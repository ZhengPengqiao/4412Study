KERN_DIR = /home/zpq/WorkPlatfrom/tiny4412/linux-3.5
TARGET := tiny4412_leds
obj-m	+= tiny4412_leds.o

all:
	make -C $(KERN_DIR) M=`pwd` modules
	arm-linux-gcc -o led_test led_test.c 

clean:
	make -C $(KERN_DIR) M=`pwd` modules clean
