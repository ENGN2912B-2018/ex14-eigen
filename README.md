# Eigen linear algebra library

Eigen is an external (3rd party) linear algebra.

## Installation on CCV
The `Eigen` package is available through the pyModules package manager on the CCV.  To load the library, you simply need to add the following line to your `.modules` file, or run it directly from the command line.

```
load eigen
```

To see the directory where Eigen include source files are located, you can run

```
show eigen
```

You will notice that the include directories are mapped to an environmental variable `EIGEN3_INCLUDE_DIR`.  This variable can be used directyl on the command line when building programs that include `Eigen` in the source file.

## Compiling programs with the Eigen library

The library may be invoked using the `-I` option directly from `g++`.

```
g++ -I ${EIGEN3_INCLUDE_DIR} main.cpp -o main
```
