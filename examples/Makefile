# options
CC = gcc
CFLAGS = -Wall -g -Og -O0
LDFLAGS = -Og
LIB = ../src
OBJS = examples.o
EXEC = result

$(EXEC): $(OBJS) $(LIB)/visualize-c-memory.so
	$(CC) $(OBJS) -o $(EXEC) $(LDFLAGS)

$(LIB)/visualize-c-memory.so: $(LIB)/visualize-c-memory.c
	$(MAKE) -C $(LIB) visualize-c-memory.so

clean:
	rm -f $(OBJS) $(EXEC)
