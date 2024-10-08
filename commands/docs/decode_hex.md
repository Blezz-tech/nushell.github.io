---
title: decode hex
categories: |
  formats
version: 0.97.1
formats: |
  Hex decode a value.
usage: |
  Hex decode a value.
---
<!-- This file is automatically generated. Please edit the command in https://github.com/nushell/nushell instead. -->

# `decode hex` for [formats](/commands/categories/formats.md)

<div class='command-title'>Hex decode a value.</div>

## Signature

```> decode hex {flags} ...rest```

## Parameters

 -  `...rest`: For a data structure input, decode data at the given cell paths


## Input/output types:

| input        | output       |
| ------------ | ------------ |
| list\<string\> | list\<binary\> |
| record       | record       |
| string       | binary       |
| table        | table        |
## Examples

Hex decode a value and output as binary
```nu
> '0102030A0a0B' | decode hex
Length: 6 (0x6) bytes | printable whitespace ascii_other non_ascii
00000000:   01 02 03 0a  0a 0b                                   •••__•

```

Whitespaces are allowed to be between hex digits
```nu
> '01 02  03 0A 0a 0B' | decode hex
Length: 6 (0x6) bytes | printable whitespace ascii_other non_ascii
00000000:   01 02 03 0a  0a 0b                                   •••__•

```
