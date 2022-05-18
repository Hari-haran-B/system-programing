#macro section
COM = g++
BIN = bin/
OBJ = object/
INC = inc/
SRC = source/
CFLAG = -c
OFLAG = -o

#target section
all: build-server build-client

#build-server target to build server binary 
build-server: compile-func 
	${COM} ${OFLAG} ${BIN}server10 ${SRC}server.cpp ${OBJ}func.o
compile-func:
	${COM} ${CFLAG} ${OFLAG} ${OBJ}func.o ${SRC}func.cpp

#build-client target to build client binary
build-client: 
	${COM} ${OFLAG} ${BIN}client10 ${SRC}client.cpp

#targets to run the program
ss:
	./${BIN}server10
sc:
	./${BIN}client10

#target to clean the bin/ and obj/ directory
clean:
	rm ${OBJ}func.o ${BIN}server10 ${BIN}client10

#end of makefile

