This is a standalone version of libbacktrace.

libbacktrace prints stack traces.

libbacktrace was originally writen by Ian Lance Taylor as part of GCC.

Building libbacktrace requires CMake.


To build for use with machinekit on debian:

   sudo apt-get install libdw-dev cmake
   
   git clone git://github.com/mhaberler/libbacktrace.git
   
   mkdir build
   
   
   cd build
   
   cmake -G'Unix Makefiles' -DENABLE_LIBBACKTRACE_TEST=true ../libbacktrace
   
   make

   # verify the library works:
   
   ./btest


   # then
   
   sudo make install
   
then run src/configure again in the machinekit directory, and rebuild.


