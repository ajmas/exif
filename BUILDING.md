Building on MacOS X with MacPorts
---------------------------------

Following represent the approach used when using MacOS X 10.12:

- Install the following dependencies, via MacPorts:

    automake, autoconf, libtool, popt, libexif

- Set the following envrionment variables:
  
        export POPT_CFLAGS=-I/opt/local/include
        export POPT_LIBS="-L/opt/local/lib -lpopt"
    
- Ensure you are in the project directory
  
- Generate the configure script. Run:
  
        autoreconf -fvi
  
- Run (default install path is /usr/local):
  
        ./configure
  
- Now build the tool:
  
        make
    
- To install:
  
        make install
 
 

