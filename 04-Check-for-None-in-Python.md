# [Check for None (Null) in Python](https://egghead.io/lessons/python-check-for-none-null-in-python)

## Null in Python

Null in Python is represented as `None`.

`foo = None`

## How to Check for Null in Python

We can check if a varaible is equal to `None` by using the `is` operator.

```python
foo = None
if foo is None:
    print"It's not there")
```

We could also check by doing `if foo == None`.

``` python
if foo == None:
    print("it's still not there")

```

Even though both mehtods give us the same results, it's better to use the `is` operator because it's faster. Why is `is` faster?

Everything in Python has an `ID` and a value. We can see this by looking at the results of `id(foo)`.

```python
id(foo)
```

This is important because the `is` operator does an ID comparison while `==` does a dict look up and has to iterate through each item in that dict to do the comparison. This means that `is` is faster.
