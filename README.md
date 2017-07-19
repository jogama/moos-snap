# MOOS snap

This is a snap of MOOS, MOOS Essentials, and MOOS Geodesy. You can also use it
for building MOOS clients simply by adding the snap itself to CMake's module
search path. For example, if you're running cmake by hand:

    $ mkdir build
    $ cd build
    $ cmake -DCMAKE_PREFIX_PATH=/snap/moos/current <path to src>

Or perhaps you're building MOOS-IvP. You can skip building IvP's bundled MOOS
and jump straight to building IvP (assuming you have its dependencies
installed:

    $ export CMAKE_PREFIX_PATH=/snap/moos/current
    $ ./build-ivp.sh
