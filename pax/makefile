CC = clang
	
INCLUDES = -I.

SRCS = ar_io.c ar_subs.c buf_subs.c cache.c  cpio.c file_subs.c ftree.c gen_subs.c getoldopt.c options.c pat_rep.c pax.c pax_format.c sel_subs.c tables.c tar.c tty_subs.c

OBJS = $(SRCS:.c=.o)

MAIN = cpio

$(MAIN): $(OBJS)
	$(CC) $(INCLUDES) -o $(MAIN) $(OBJS)

.c.o:
	$(CC) $(CFLAGS) $(INCLUDES) -c $<  -o $@

clean:
	$(RM) *.o *~ $(MAIN)

