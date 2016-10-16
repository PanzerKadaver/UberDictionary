CC = gcc
RM = rm -f
BIN = etape1

SRCS = main.c \

OBJS = $(SRCS:.c=.o)

CFLAGS = -I. -I./include/
CFLAGS += -W -Wall -Wextra -g
LDFLAGS += -lpthread

all: $(BIN)

$(BIN) : $(OBJS)
	$(CC) -o $(BIN) $(OBJS)

clean :
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(BIN)

debug: CFLAGS += -g
debug: re

re: fclean all

run: debug
	etape1 $(ARGS)
