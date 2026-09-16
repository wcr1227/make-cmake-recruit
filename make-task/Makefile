CC = gcc
CFLAGS = -Wall -Wextra -Iinclude

calculator: main.o calculator.o logger.o
	# TODO1: link object files into the calculator executable
	$(CC) main.o calculator.o logger.o -o calculator

main.o: src/main.c include/calculator.h include/logger.h
	# TODO2: compile src/main.c
	$(CC) $(CFLAGS) -c src/main.c -o main.o

calculator.o: src/calculator.c include/calculator.h
	# TODO3: compile src/calculator.c
	$(CC) $(CFLAGS) -c src/calculator.c -o calculator.o

logger.o: src/logger.c include/logger.h
	# TODO4: compile src/logger.c
	$(CC) $(CFLAGS) -c src/logger.c -o logger.o

.PHONY: clean
clean:
	# TODO5: remove calculator and all .o files
	rm -f calculator *.o