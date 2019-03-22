# Name: Aidan Tribble
# Course: CIS145 Intro to DevOps
# CRN: 45595
# Date: 01.29.2019
# Assignment: Make - Write a Makefile to Compile C Code

runCount3s: Count3s
	./Count3s

Count3s: countThrees.o readInt32BitLE.o
	gcc -Wall countThrees.o readInt32BitLE.o -o Count3s

countThrees.o:
	gcc -c -Wall countThrees.c

readInt32BitLE.o:
	gcc -c -Wall readInt32BitLE.c

clean:
	-rm -f *.o Count3s
