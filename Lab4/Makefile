CC=gcc
CFLAGS=-Iinclude
DEPS = mylibrary.h
OBJ = src/mylibrary.o src/main.o 

%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

myproject: $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS)

.PHONY: clean

clean:
	rm -f src/*.o myproject
