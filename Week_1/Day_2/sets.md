# Skills required to be a data scientist

[Article](https://dimensionless.in/is-programming-knowledge-required-to-pursue-data-science/)

# Python tips

('''
hello 
 ''')

This created a docstring or a block comment if you look at the code.

Long lines of code should be shortened by using tab and brackets to enhance 
readability 

``` python
>>> a = [
...     [1, 2, 3, 4, 5],
...     [6, 7, 8, 9, 10],
...     [11, 12, 13, 14, 15],
...     [16, 17, 18, 19, 20],
...     [21, 22, 23, 24, 25]
... ]
```


# Sets
Used for data that will be present only once. 

Sets [link](https://realpython.com/python-sets/)

In Sum
* sets are unordered
* sets have no duplicates
* elements inside a set are immutable
* sets can be defined with set() or {}
    * set('foo') will iterate through the string
        * output = f , o 
    * {'foo'} will treat foo as 1 iteration
        * output = 'foo'
* lists and dictionaries cannot be added into a set
* to combine sets use | or .union()
    * | requires both to be sets while union() converts the input to a set
* intersection() method finds common values in 2 sets
* difference() method finds values only in 1 of the sets
* symmetric_difference() method finds values opposite of intersection()
    * can use ^ operator instead to include multiple sets

``` python
>>> a = {1, 2, 3, 4, 5}
>>> b = {10, 2, 3, 4, 50}
>>> c = {1, 50, 100}

>>> a ^ b ^ c
{100, 5, 10}
```

* isdisjoint() returns true if no values are in common between multiple sets

### Modifying sets

* .update or |= to add elements
* .intersection_update() or &= to retain intersecting values
* .difference_update() or -= to find values found only in 1 set
* .symmetric_difference_update() or ^=
* add()
* discard()
* pop() removes a random element from the set because sets are unordered
* frozensets are the same as sets except they're immutable
    * defined with frozensets()