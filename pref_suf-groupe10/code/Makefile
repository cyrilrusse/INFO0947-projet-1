### 
## Makefile
## INFO0947: Projet 1
## 
## RUSSE Cyril
### 

## Variables

# Tools & flags
CC=gcc
CFLAGS=--std=c99 --pedantic -Wall -W -Wmissing-prototypes
LD=gcc
LDFLAGS=

# Files
EXEC=prefixe_suffixe
MODULES=main.c prefixe_suffixe.c
OBJECTS=main.o prefixe_suffixe.o

## Rules

all: $(EXEC)

prefixe_suffixe: $(OBJECTS)
	$(LD) -o $(EXEC) $(OBJECTS) $(LDFLAGS)

main.o: main.c
	$(CC) -c main.c -o main.o $(CFLAGS)

prefixe_suffixe.o: prefixe_suffixe.c
	$(CC) -c prefixe_suffixe.c -o prefixe_suffixe.o $(CFLAGS)

clean:
	rm -f *.o $(EXEC) *~