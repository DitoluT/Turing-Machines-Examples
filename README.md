# Turing Machines in JFLAP

In this repository you will find several examples of Turing machines implemented using JFLAP (https://www.jflap.org/).

## Language 1

In the `Language 1` folder you will find a Turing machine that accepts the language:

L1 = { 0^(2^n) | n >= 0 }

That is, the machine accepts strings composed only of `0`s whose length is a power of 2 (e.g., 1, 2, 4, 8, 16, ...).

The machine works by repeatedly checking whether the number of symbols can be evenly divided by 2 until a single symbol remains.

## Language 2

In the `Language 2` folder you will find a Turing machine that accepts the language:

L2 = { #x1#x2#...#xl | each xi ∈ {0,1}* and xi ≠ xj for all i ≠ j }

This language consists of a sequence of binary strings separated by `#`, where **all substrings are pairwise different**.

### Valid examples:
- `#0#1#01#`
- `#10#11#00#01#`

### Invalid examples:
- `#0#1#0#` (repeated substring)
- `#01#10#01#` (duplicate `01`)

The Turing machine checks that no substring appears more than once by comparing each string with the others.
