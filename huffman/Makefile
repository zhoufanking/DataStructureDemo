CFLAGS=-O2 -Wall -Werror
#CFLAGS=-g -Wall -Werror
CC=gcc

all: huffcode libhuffman.a

huffcode: huffcode.o libhuffman.a
	$(CC) -o $@ huffcode.o libhuffman.a

huffman.o: huffman.h

libhuffman.a: huffman.o
	$(AR) r $@ $<

clean:
	$(RM) *.o *~ core huffcode libhuffman.a
