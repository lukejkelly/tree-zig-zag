CFLAGS=-Wall -Wextra -O3 -I$$(brew --prefix)/include -std=c++17
LDFLAGS= -lgsl -lgslcblas -lconfig++ -L$$(brew --prefix)/lib
CC = g++


main: simulate.cc
	${CC} ${CFLAGS} -o simulate simulate.cc ${LDFLAGS}

gen: gen_data.cc
	${CC} ${CFLAGS} -o gen_data gen_data.cc ${LDFLAGS}
