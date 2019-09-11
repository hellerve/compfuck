# compfuck

Brainfuck translated to Carp at compile time. Just add `(compf "<brainfuck code>")` to
your program, and the equivalent Carp code will be emitted and compiled into your program.

## Wat

Basically, this is a quick example macro that proofs that the compile-time environment of
Carp is quite capable of emitting complex code. This program in particular uses
string-based code emission, meaning that we analyze the source and emit Carp code based on
it. I don’t expect this to be very fast, but that’s not the point.

Ultimately, there is no point.

## Usage

```clojure
(load "compfuck.carp")

; print the ascii charset and then some
(compf "+[+.]")
```

<hr/>

Have fun!
