CC=gcc 
CFLAGS=-Wall -lwiringPi -lwiringPiDev
app=example

all: link

link: compile 
	gcc -o $(app) $(app).o $(CFLAGS)
	rm -f $(app).o

compile: $(app).c
	gcc -c $(app).c	
	
clean:
	rm -f $(app) $(app).o
run: $(app)
	./$(app)
