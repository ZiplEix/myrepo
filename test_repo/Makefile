##
## EPITECH PROJECT, 2021
## Makefile
## File description:
## Project's main makefile
##

SRC	=	$(wildcard *.c) $(wildcard src/*.c)

OBJ	=	$(SRC:.c=.o)

NAME	=	minishell2

TESTS	=	-lcriterion --coverage

LIB     =	-L./lib -llibrary

${NAME}:	${OBJ}
			make -C./lib/
			make -C./lib/library
			gcc -o ${NAME} ${OBJ} $(LIB)

all :		${NAME}

clean:
			rm -f ${OBJ}
			make clean -C./lib/
			make clean -C./lib/library


fclean:	clean
			rm -f ${NAME}
			make fclean -C./lib/
			make fclean -C./lib/library


re:		fclean all

.PHONY: all clean fclean re
