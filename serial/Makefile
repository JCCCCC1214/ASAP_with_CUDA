CC = gcc
CFLAG = -O3 -I../common
LFLAG = -lm

EXE = serial
SRC = serial.c

OBJ = ${SRC:.c=.o}

all: ${EXE}

${EXE}: ${OBJ}
	${CC} $^ ${CFLAG} -o $@ ${LFLAG}

%.o: %.c
	${CC} ${CFLAG} -c $^ -o $@

.PHONY: clean

clean:
	rm -rf ${EXE} ${OBJ} 