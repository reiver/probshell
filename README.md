# probshell

**probshell** is a simple *probability calculator*.

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

