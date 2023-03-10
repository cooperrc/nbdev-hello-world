nbdev-hello-world
================

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

This is a simple dice throwing class that uses [NumPy
default_rng](https://numpy.org/doc/stable/reference/random/generator.html)
to build an array of random integers depending upon the number of sides
on the dice and the number of dice thrown.

## Install

``` sh
pip install nbdev-hello-dice
```

## How to use

Here, we throw 1 die with 6 sides:

``` python
result = throw(6)
result
```

    1 = sum([1])

Next, we can throw $\times 2$ dice and look at the sum

``` python
throw(6, 2)
```

    3 = sum([1 2])

The dice values are stored in an array, as `throw(N, inhand).dice` as
such

``` python
result = throw(6, 4)
result.dice
```

    array([2, 1, 4, 6])

The `sum` of the dice values are saved in `throw.(N, inhand).sum` as
such

``` python
result.sum
```

    13
