---
title: random chars
categories: |
  random
version: 0.97.1
random: |
  Generate random chars uniformly distributed over ASCII letters and numbers: a-z, A-Z and 0-9.
usage: |
  Generate random chars uniformly distributed over ASCII letters and numbers: a-z, A-Z and 0-9.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `random chars` for [random](/commands/categories/random.md)

<div class='command-title'>Generate random chars uniformly distributed over ASCII letters and numbers: a-z, A-Z and 0-9.</div>

## Signature

```> random chars {flags} ```

## Flags

 -  `--length, -l {int}`: Number of chars (default 25)


## Input/output types:

| input   | output |
| ------- | ------ |
| nothing | string |

## Examples

Generate a string with 25 random chars
```nu
> random chars

```

Generate random chars with specified length
```nu
> random chars --length 20

```
