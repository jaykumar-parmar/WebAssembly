#Compiler
COMPILER = g++

#Compiler flags
CFLAGS = -o

#Linker Flags
LINKER = $(COMPILER) $(CFLAGS)

#Objects Files
OBJS = add.o substract.o

#Target File
PROG = mathlib.lib

#Make all target
all: $(PROG)

#Execution
$(PROG) : $(OBJS)
	$(LINKER) $(PROG) $(OBJS) -shared


%.o : %.cpp
	$(COMPILER) -c $< -o $@ -shared


#Dependency
add.o	: add.cpp
substract.o	: substract.cpp
