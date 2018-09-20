Create a directory build:

> mkdir build;

Go into that directory

> cd build;

You can choose to build a release version with:

> cmake ../ -DCMAKE_BUILD_TYPE=Release

or a debug version with

> cmake ../ -DCMAKE_BUILD_TYPE=Debug

And build everything with

> make

Test matrix multiplication

> ./tester -t Matrix -r detailed 

Test Crout and Doolittle methods, the unpacking* methods and matrix inversion

> ./tester -t LU -r detailed

Tests the QR method, check if Q is orthogonal, R is upper triangular and QR=A

> ./tester -t QR -r detailed
