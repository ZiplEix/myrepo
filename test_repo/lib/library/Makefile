##
## EPITECH PROJECT, 2022
## test_repo
## File description:
## Makefile for lib library.
##

SRC=	$(wildcard *.c)

NAME=	liblibrary.a

LIB_DEST=	../

OBJ=	$(SRC:.c=.o)

all:	$(NAME)

$(NAME):	$(OBJ)
	ar rc $(NAME) $(OBJ)
	cp $(NAME) $(LIB_DEST)

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)
	rm -f ../$(NAME)

re: fclean all
