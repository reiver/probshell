# probshell

**probshell** is a simple *probability calculator*, with a command-line interface (CLI)

(I have seen some people call this type of thing a REPL (read–eval–print loop).)

_probshell_ also supports _exporting_ and _importing_, so that it has a kind of scripting language;
although perhaps it would be more accurate to describe it as a (text-based) database.

## Example
Here is an example _probshell_ session:
```
¿> P(H):=0.01
¡ P(H):=1/100
∴ P(¬A)=99/100

¿> P(D|H):=0.9
¡ P(D|H):=9/10
∴ P(¬D|H)=1/10

¿> P(¬D|¬H):=0.9
¡ P(¬D|¬H):=9/10
∴ P(D|¬H)=1/10
∴ P(D)=27/250
∴ P(¬D)=223/250
∴ P(H|D)=1/12
∴ P(¬H|D)=11/12
∴ P(H|¬D)=1/892
∴ P(¬H|¬D)=891/892

¿> exit
```

## Notation

Here are some example _probshell_ notation, that illustrates the different ways that numbers can be written:
```
P(A):=1
```

```
P(B):=0
```

```
P(C):=0.3
```

```
P(D):=1/3
```

(Note that the ":=" symbol is being used, and not just the "=" symbol. The latter will *not* work.)


Here we see that there are 4 different ways of denoting numbers:
* the _whole number_ one (1),
* the _whole number_ zero (0),
* the _decimal numbers_ (such as 0.3, 0.02, 0.577215664901, 0.0000000000000003, etc)
* and _fractions_ (such as 1/2, 1/3, 7/22, 17699/125000, etc)

### Complement

There is also a way of *complementing* -- i.e., *negating* -- statement variables.
There are actually 4 different ways of doing this, shown in the following examples:
```
P(~A):=0.9
```

```
P(!A):=0.9
```

```
P(-A):=0.9
```

```
P(¬A):=0.9
```

(The last method is the canonical method. However, since not all keyboard have the "¬" character, the other methods are made available.)

### Conditional

The notation also supports _conditional probabilities_. You can see this in the following example:
```
P(D|H):=0.8
```

Negation is also supported for conditional probabilities, as in:
```
P(¬W|C):=0.7
```

```
P(~G|~F):=2/3
```

