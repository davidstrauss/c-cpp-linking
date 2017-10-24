# C to C++ Linking with Meson

## Building

1. Set up build system:

       meson builddir

1. Then, either perform a normal build:

       ninja -C builddir

1. Or, use Clang Analyzer:

       ninja scan-build -C builddir

## Running

* Run normally:

       builddir/demo

* Run under Valgrind:

       valgrind --leak-check=yes builddir/demo
