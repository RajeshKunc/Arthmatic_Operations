# Compiler
CC = gcc

# Flags
CFLAGS = -Wall -g
CFLAGS += -I../Includes

# Target executable
TARGET = myapp

# Source files
SRCS = main.c addition.c subtraction.c multiplication.c division.c

# Object files (auto convert .c → .o)
OBJS = $(SRCS:.c=.o)

# Default target
$(TARGET): $(OBJS)
	$(CC) $(OBJS) -o $(TARGET)

# Rule to compile each .c → .o
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Clean rule
clean:
	rm -f $(OBJS) $(TARGET)
