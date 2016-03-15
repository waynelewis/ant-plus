CC = g++
RM = /bin/rm -f

TOP = /Users/wlewis/local/data/personal/code/git/repos/ant+/lib/ANT_Library_MacOSX_Package/ANT_Library_MacOSX_Package

CFLAGS = -g
INCFLAGS += -I$(TOP)/ANT_LIB/inc

all: demo

demo: libant.o demo.o
	$(CC) $(CFLAGS) -o demo \
		libant.o \
		demo.o \
		$(LDFLAGS)

%.o: %.cpp %.h
	$(CC) -c $(INCFLAGS) $< -o $@ 
