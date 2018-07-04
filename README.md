trusting
========

Run a command trusting that it will succeed, squelching `stdout` and
`stderr`. If errors do occur, i.e. the command exists with a non-zero
exit code, the full `stdout` and `stderr` output will be printed after
that error has occurred.

`trusting` requires Python 3.5 or greater.

Usage
-----

Assuming `trusting` is somewhere in your `PATH`,

	$ trusting pdflatex doc.tex

will run `pdflatex doc.tex` without all that verbose output you don't
want to see.

Limitation
----------

Because `stdin` is set to `/dev/null`, user input for the running
commands are not supported.
