PROGS =		runDynamic
CFLAGS +=	-Wall
LDLIBS +=	-lusb-1.0
CC =		gcc
LD =		${CC}

all: ${PROGS}

%.o: %.c
	${CC} ${CFLAGS} -c $<

%: %.o
	${LD} ${LDFLAGS} -o $@ $< ${LDLIBS}

clean:
	-rm -f ${PROGS} *.o
