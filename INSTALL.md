# INSTALL

## 1 Introduction

If you are installing this package as part of the GNUstep core packages,
read the file GNUstep-HOWTO for more complete instructions on how to
install the entire GNUstep package (including this library).
GNUstep-HOWTO is located in the gnustep-make package or at
`http://www.gnustep.org'

   This version of gnustep-boron requires:

   * gnustep-make version 2.0.0 or higher
   * a working C++ compiler

   On libstdc++-based operating systems, such as most GNU/Linux systems, 
   this version also requires a copy of the libstdc++ and g++ header files
   of the same version as the GCC that Clang discovers. Run `clang-14 -v`
   to find out which version of libstdc++ and g++ you need to install.

If you are installing the GNUstep libraries individually, make sure
you already have the GNUstep Makefile package (gnustep-make) installed,
and you have sourced the makefile script:
   . $GNUSTEP_SYSTEM_ROOT/Library/Makefiles/GNUstep.sh

Quick installation instructions:

   ./configure
   make
   make install

## 2 Configuration

Configuration is performed by running the `configure' program at a
shell prompt. You may want to use some of the optional arguments to the
`configure' program. Type `configure --help' for a list of these. It is
not likely that you will need to use the `--prefix' option, since
gnustep-boron will automatically install in the directory specified by
the `GNUSTEP_SYSTEM_LIBRARY' environment variable (specified when you
installed gnustep-make).

## 3 Compilation

To compile this library, type 'make'. After this is complete, type 'make
install' (you must be the root user). Some additional options you
can use with make are `debug=yes' to make a debugging version of the
library and `shared=no' to make a static version of the library. See
the gnustep-make package for more information on these options.



  Copyright (C) 2017 Free Software Foundation

  Copying and distribution of this file, with or without modification,
  are permitted in any medium without royalty provided the copyright
  notice and this notice are preserved.
