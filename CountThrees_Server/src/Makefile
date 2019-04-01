# Name: Aidan Tribble
# Course: CIS145 Intro to DevOps
# CRN: 45595
# Date: 02.15.2019
# Assignment: 03 XLab: Makefile - Build and Launch ServerCountThrees

all: ServerCountThrees test

test: | build
	cp ServerCountThrees ../data/threesData.bin -t ../build
	./ServerCountThrees

build:
	mkdir -p ../build

ServerCountThrees: ServerCountThrees.o readInt32BitLE.o
	gcc -Wall ServerCountThrees.o readInt32BitLE.o -o ServerCountThrees

ServerCountThrees.o:
	gcc -c -Wall ServerCountThrees.c

readInt32BitLE.o:
	gcc -c -Wall readInt32BitLE.c

clean:
	rm -f *.o ServerCountThrees
	rm -rf ../build
