PROG=	spfwalk
SRCS=	spfwalk.c dns.c event_asr_run.c
MAN=	spfwalk.1
#NOMAN=

CFLAGS+= -I.
CFLAGS+= -Wall
CFLAGS+= -D'pledge(x,y)=0'
LDLIBS=	-levent -lasr

all: $(PROG)

clean:
	rm -f $(PROG) *.o

$(PROG): $(SRCS:.c=.o)
