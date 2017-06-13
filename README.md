# freebsd-cross-build

This creates a container that can be used to build FreeBSD binaries
natively on Linux

To build:

    ./build

(this finishes by running 'docker build -t freebsd-cross-build .')

To run:

    docker run --rm -it freebsd-cross-build

There is /freebsd/bin on the path. It has all of the build
tools (e.g. x86_64-pc-freebsd9-gcc)

It is likely you would add a -v switch to the run (to put your
code on a mount).
