RM=rm -f
CPPFLAGS= -I /usr/local/jansson/include -I ./nanoflann/include -I ../../common
LDFLAGS= -static-libgcc
LDLIBS=/usr/local/jansson/lib/libjansson.a

all: ExtractPGA 

ExtractPGA.o : ExtractPGA.cpp

ExtractPGA: ExtractPGA.o
	$(CXX) $(LDFLAGS) -o ExtractPGA ExtractPGA.o $(LDLIBS)

clean:
	$(RM) *.o *~

distclean: clean
	$(RM) ExtractPGA


