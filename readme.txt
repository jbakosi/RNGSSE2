
To compile the library:

  cd source
  make

To compile, for example, "mrg32k3a.c" in the current directory, with use of the library:

  gcc -o mrg32k3a mrg32k3a.c -I../../include -L../../lib -lrngsse

To compile all the examples in C in the current directory, with use of the library:

  bash -c 'for i in *.c; do gcc -o ${i%??} $i -I../../include -L../../lib -lrngsse; done'

To compile all the examples in FORTRAN in the current directory, with use of the library:

  bash -c 'for i in *.f90; do gfortran -o ${i%????} $i -L../../lib -lrngsse; done'

