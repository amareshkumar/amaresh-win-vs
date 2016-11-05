CC = g++
#CXXFLAGS = -std=c++0x -std=c++11 -std=gnu++11 -std=gnu++0x -g -o2 -pedantic -I/cygdrive/d/pro/code/linux/inc -DINTERACTIVE
CXXFLAGS = -std=c++11 -g -pedantic -I/cygdrive/d/pro/code/linux/inc
object := $(patsubst %.cpp,%.o, $(wildcard *.cpp))

all: amaresh
	cp amaresh ../
amaresh: $(object)
	#cc $(CXXFLAGS) -o amaresh $(object) -lstdc++ -L/usr/ -L/usr/lib -L/usr/local/bin
	$(CC) $(CXXFLAGS) $(object) -lstdc++ -lpthread -L/usr/ -L/usr/lib -L/usr/local/bin -o amaresh 
clean: 
	rm -f *.o amaresh amaresh.exe