

- Create ML
- MLBoundingBoxUnits
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value indicating whether two values are equal.

macOS 10.15+

``` source
static func == (a: MLBoundingBoxUnits, b: MLBoundingBoxUnits) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Equality is the inverse of inequality. For any values `a` and `b`, `a == b` implies that `a != b` is `false`.

## See Also

### Comparing errors

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

