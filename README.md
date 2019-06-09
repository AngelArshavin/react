React — Declarative events and signals for OCaml
-------------------------------------------------------------------------------
Release %%VERSION%%

React is an OCaml module for functional reactive programming (FRP). It
provides support to program with time varying values : declarative
events and signals. React doesn't define any primitive event or
signal, it lets the client chooses the concrete timeline.

React is made of a single, independent, module and distributed under
the BSD3 license.

## Installation

React can be installed with `opam`:

    opam install react

If you don't use `opam` consult the [`opam`](opam) file for build
instructions.


## Documentation

The documentation and API reference is automatically generated by
`ocamldoc` from the interfaces. It can be consulted [online][3]
and there is a generated version in the `doc` directory of the 
distribution. 

[3]: http://erratique.ch/software/react/doc/React


## Sample programs

If you installed React with `opam` sample programs are located in
the directory `opam config var react:doc`.

In the distribution sample programs are located in the `test`
directory of the distribution. They can be built with:

    ocamlbuild -use-ocamlfind test/tests.otarget

The resulting binaries are in `_build/test`.

- `test.native` tests the library, nothing should fail.
- `clock.native` is a command line program using ANSI escape sequences 
  and the Unix module to print the current local time. 
- `breakout.native` is a command line program using ANSI escape sequences
  and the Unix module to implement a simple breakout game.
