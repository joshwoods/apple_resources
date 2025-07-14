

- App Store Connect API
- Game Center
- Expressions
-  Intersecting sets 

Article

# Intersecting sets

Return the intersection of two or more arrays treated as sets.

## Overview

Use the `intersection()` function in the expression of a matchmaking rule to find the common items in arrays. For example, intersection `([[ ‘a’, ‘b’ ], [ ‘b’, ‘c’ ], [ ‘b’, ‘d’]])` returns `[ ‘b’ ]`.

### Declaration

```
array intersection(array[array[any]] $sets)
```

### Parameters

`sets`  
An array of arrays that the function converts to sets and then intersects with each other.

### Return value

A set that’s the intersect of the set representation of the arrays in `sets`.

## See Also

### Array functions

Converting arrays to sets

Return the content of a list, with duplicates removed and sorted, so that you can compare it to another set.

Computing numeric differences

Return the absolute difference between the maximum and minimum numerical values in an array.

