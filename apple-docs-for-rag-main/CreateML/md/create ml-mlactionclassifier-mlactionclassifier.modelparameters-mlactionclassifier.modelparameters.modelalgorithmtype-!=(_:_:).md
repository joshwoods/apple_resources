

- Create ML
- MLActionClassifier
- MLActionClassifier.ModelParameters
- MLActionClassifier.ModelParameters.ModelAlgorithmType
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

Create MLSwiftmacOS 10.14+

``` source
static func != (lhs: Self, rhs: Self) -> Bool
```

## Parameters 

`lhs`  

A value to compare.

`rhs`  

Another value to compare.

## Discussion

Inequality is the inverse of equality. For any values `a` and `b`, `a != b` implies that `a == b` is `false`.

This is the default implementation of the not-equal-to operator (`!=`) for any type that conforms to `Equatable`.

## See Also

### Comparing algorithm types

static func == (MLActionClassifier.ModelParameters.ModelAlgorithmType, MLActionClassifier.ModelParameters.ModelAlgorithmType) -> Bool

Returns a Boolean value indicating whether two values are equal.

