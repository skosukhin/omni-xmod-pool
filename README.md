# OMNI xmod pool

[![Build Status](https://travis-ci.org/claw-project/omni-xmod-pool.svg?branch=master)](https://travis-ci.org/claw-project/omni-xmod-pool)

Sets of generic xmod file for OMNI Compiler

## Building .xmod files using F_Front

Use the `F_Front` binary of the claw installation and a Fortran file in order to create a `.xmod` file. **Careful:** if your file depends on other modules, they also have to be transformed into `.xmod` before being 
able to be read by the F_Front! Include module dependencies using the -M option and -I option for headerdependencies:

    $ ./F_Front code.f90 -M [.xmod dirpath] -I [.h dirpath]

