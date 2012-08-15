
#-----------------------------------------------------------------------------
# Make rules:
#-----------------------------------------------------------------------------
all: test1

test1:
	gcc -mavx -O3 -c test1.c -std=c99 -fopenmp && gcc -mavx -O3 -S -fverbose-asm test1.c -std=c99 -fopenmp && gcc -lgomp -fopenmp -o test1 test1.o

run:
	./test1 1000000

clean:
	rm test1
