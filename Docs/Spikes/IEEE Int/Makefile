SOURCE = program.c
SOURCE_O = program.o
PROGRAM = program
CFLAGS = -Wall -pedantic -std=c11

run: ${PROGRAM}
	./${PROGRAM}

${PROGRAM}: ${SOURCE_O}
	gcc -o ${PROGRAM} ${SOURCE_O} -lm

${SOURCE_O}: ${SOURCE}
	gcc ${CFLAGS} -c ${SOURCE}

clean: 
	rm -rf *.o *.out ${PROGRAM}
