
##
 # startup code provided by Paul Miller for COSC1114 - Operating Systems
 # Principles
 ##

# provide make targets here to build the two programs 

.default: all

all: 
	copier
	mtcopier

clean:
	rm -rf copier mtcopier *.o *.dSYM

copier: copier_files/main.cpp copier_files/reader.cpp copier_files/writer.cpp
	g++ -Wall -Werror -std=c++20 -g -O -o $@ $^

mtcopier: mtcopier_files/main.cpp mtcopier_files/reader.cpp mtcopier_files/writer.cpp
	g++ -Wall -Werror -std=c++20 -g -O -o $@ $^

%.o: %.cpp
	g++ -Wall -Werror -std=c++20 -g -O -c -o $@ $<