
CROSS_COMPILE ?= arm-linux-androideabi-
CC := $(CROSS_COMPILE)gcc
LD := $(CROSS_COMPILE)ld

LIB_DIR := ../install
CFLAGS += -I ../install/include/
CFLAGS += -lm

all: minesweeper

minesweeper: minesweeper.c
	$(CC) minesweeper.c $(CFLAGS) ../install/lib/libminigui_ths.a -o minesweeper

clean:
	rm -rf minesweeper *.o
