# options
CC = gcc
CFLAGS = -Wall -g -fpic -Og
LDFLAGS = -shared -Og

OBJS = visualize-c-memory.o
LIB = visualize-c-memory.so

$(LIB): $(OBJS)
	$(CC) $(OBJS) -o $(LIB) $(LDFLAGS)

clean:
	rm -f $(OBJS) $(LIB)
