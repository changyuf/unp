include ../Make.defines

SRCS=Error.cc Utility.cc SocketWrapper.cc StdioWrapper.cc ReadLine.cc UnixWrapper.cc

OBJS=$(SRCS:.cc=.o)

LIBUNP_NAME = ../lib/libunp.a

all:    ${OBJS}
	ar rv ${LIBUNP_NAME} $?
	${RANLIB} ${LIBUNP_NAME}

clean:
	\rm -rf ${CLEANFILES} ${LIBUNP_NAME}
