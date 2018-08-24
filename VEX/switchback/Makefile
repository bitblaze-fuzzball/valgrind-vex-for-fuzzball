
#CC=aarch64-linux-gnu-gcc

all: switchback.c linker.c linker.h
	$(CC) -m64 -Wall -O -g -o switchback switchback.c linker.c \
		../libvex.a test_hello.c

test_ppc:
	$(CC) -Wall -m64  -mregnames -O -c test_ppc_jm1.c

clean:
	rm -f switchback switchback.o linker.o
