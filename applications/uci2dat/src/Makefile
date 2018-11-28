#
# Copyright (C) 2018 Willy All rights reserved
#
# Written by Willy(jasenwan@163.com)
# Created Time: Wed 28 Nov 2018 01:07:42 PM CST
#

TARGET=uci2dat
OBJS=uci2dat.o

.c.o:
	$(CC) -c $(CFLAGS) $< -o $@

all:$(TARGET)

$(TARGET):$(OBJS)
	$(CC) $(CFLAGS) $(LDFLAGS) $^ -o $@

clean:
	rm -rf *.o *.elf $(TARGET)
