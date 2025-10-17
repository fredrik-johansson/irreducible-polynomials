# Tables of irreducible polynomials

## Irreducible polynomials of minimal weight

These tables list irreducible polynomials of minimal weight (i.e. maximal sparsity) over $\textrm{GF}(p)$ for every degree $n$ up to the indicated bound, useful if one wants to do efficient arithmetic in $\textrm{GF}(p^n)$ for various large values of $n$. We give just one polynomial for each $n$, even if several candidates with the same minimal weight are available.

* [data/minimal_irreducibles_2.txt](data/minimal_irreducibles_2.txt) - $\textrm{GF}(2)$, $1 \le n \le 6000$
* [data/minimal_irreducibles_3.txt](data/minimal_irreducibles_3.txt) - $\textrm{GF}(3)$, $1 \le n \le 10000$
* [data/minimal_irreducibles_5.txt](data/minimal_irreducibles_5.txt) - $\textrm{GF}(5)$, $1 \le n \le 6000$
* [data/minimal_irreducibles_7.txt](data/minimal_irreducibles_7.txt) - $\textrm{GF}(7)$, $1 \le n \le 5000$
* [data/minimal_irreducibles_11.txt](data/minimal_irreducibles_11.txt) - $\textrm{GF}(11)$, $1 \le n \le 5000$
* [data/minimal_irreducibles_13.txt](data/minimal_irreducibles_13.txt) - $\textrm{GF}(13)$, $1 \le n \le 2000$
* [data/minimal_irreducibles_17.txt](data/minimal_irreducibles_17.txt) - $\textrm{GF}(17)$, $1 \le n \le 2000$
* [data/minimal_irreducibles_19.txt](data/minimal_irreducibles_19.txt) - $\textrm{GF}(19)$, $1 \le n \le 2000$
* [data/minimal_irreducibles_23.txt](data/minimal_irreducibles_23.txt) - $\textrm{GF}(23)$, $1 \le n \le 2000$
* [data/minimal_irreducibles_29.txt](data/minimal_irreducibles_29.txt) - $\textrm{GF}(29)$, $1 \le n \le 2000$

These tables were generated with a development version of [FLINT](https://flintlib.org) (see https://github.com/flintlib/flint/pull/2417) and can easily be extended by running the ``minimal_irreducibles`` example program.

```
$ build/examples/minimal_irreducibles -threads 8 3 1 500
p = 3, nmin = 1, nmax = 500
x
x^2 + 1
x^3 + 2 * x + 1
x^4 + x + 2
x^5 + 2 * x + 1
x^6 + x + 2
...
x^497 + x^23 + x^21 + 1
x^498 + 2 * x^118 + 1
x^499 + x^20 + 2
x^500 + x^39 + 2
cpu/wall(s): 5.587 1.044
virt/peak/res/peak(MB): 521.84 828.11 9.34 10.35
```
