#
# Makefile for Basic Unix
#
#
# Destination of executable
DESTDIR = ./
#
# ----Compiler stuff
# What compiler ... on SGI we use MIPS c
CC=cc
# Our includes are here with the source.
INC = -I./
#
#---- Processor flags - uncomment your favourite
# 1. unknown
#PROCFLAGS=
# 2. r4k
PROCFLAGS = -mips3
# 3. r5k
#PROCFLAGS = -mips4
#
# --- Libraries for Linking and stuff
#
GLUTINC = -I/usr/local/include 
GLUTLIB = -L/usr/local/lib -lglut
#
OPENGL = -lGL -lGLU
XLIBS = -lXmu -lXext -lX11
MATHLIB = -lm
#
OBJS = lesson13.o 
#
#======================================================
#
CFLAGS = $(INC) $(GLUTINC) $(PROCFLAGS)
LDLIBS = $(GLUTLIB) $(OPENGL) $(XLIBS) $(MATHLIB)

# Link phase

lesson13:     $(OBJS)
	$(CC) $(OBJS) $(CFLAGS) -o lesson13 $(LDLIBS) 

#
# Dependency list.
#
lesson13.o:	lesson13.c
