

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.FeaturePrintType
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Returns a Boolean value indicating whether two values are not equal.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

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

### Comparing feature-print types

static func == (MLSoundClassifier.ModelParameters.FeaturePrintType, MLSoundClassifier.ModelParameters.FeaturePrintType) -> Bool

Returns a Boolean value indicating whether two values are equal.

