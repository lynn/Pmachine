# P-machine interpreter

This is a fork of the P-machine interpreter used for the Compilers course at UAntwerp.

I’ve fixed [exactly one bug](https://github.com/lynn/Pmachine/commit/1578d2b5c3cff6c5f0135eec5e15f97d7976cb69#diff-e3eb7fc7b9bca70ab6b72a0eb8b4d96e), in the `sro` instruction’s implementation. 

## Instructions

Install `flex` and `bison`, then run `make`. The resulting binary is called `Pmachine`:

    USAGE: Pmachine [filename] <-s [numeric value]> <-t [numeric value]> <-h>

         -s: stepsize
         -t: number of stackplaces to show (by default all)
         -h: show heap

Try `echo 10 | ./Pmachine fibonacci.p`, for example.
