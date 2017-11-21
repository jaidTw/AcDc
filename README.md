# AcDc
AcDc is a very simple hand-crafted Ac to Dc language compiler, it's an assignment of introductory compiler course in NTU.
You may get more information about Dc language from [dc(1)](https://linux.die.net/man/1/dc).

## Specification of Ac language
### Types
There're two kind of variable types, integer and float, which is declared by `i` and `f`, each variable has to be declared before their use.

### Reserved words
There are only three reserved words, `i`, `f`, and `p`, as mentioned above, `i` and `f` are variable declarations, `p` is an opeartion for printing out the content of a variable.

### Variable
Ac accepts variable name's length up to 64 characters, allowed characters including A-Z, a-z, 0-9 and _(underscore),
and the total of variables must not exceed 23.

### Operators
There are five operators : `+`, `-`, `*`, `/`, `=`, which is addition, subtraction, multiplication, division and value assignment.

## Usage
```
$ ./AcDc <source_file> <output_file>
```

## How to build
run
```
$ make
```

## features
* support constant folding
