# makefile

The root directory contains only one makefile, the one `make` reads by default.

## Naming

Name the root makefile `Makefile`, and keep `GNUmakefile` and `makefile` out of
the root.

When running `make`, GNU Make searches for a makefile by trying these names in
order: `GNUmakefile`, `makefile`, then `Makefile`, so either of the first two
hides `Makefile`.

`Makefile` is the recommended name: in an ASCII listing, uppercase sorts before
lowercase, so it appears near the top of a directory listing, next to `README`
and `LICENSE`.

Reserve `GNUmakefile` for a file specific to GNU Make. Other implementations of
`make`, such as POSIX `make` and BSD `make`, will not understand that file, and
they do not look for the name `GNUmakefile`.

See
[Makefile Names](https://www.gnu.org/software/make/manual/html_node/Makefile-Names.html).
