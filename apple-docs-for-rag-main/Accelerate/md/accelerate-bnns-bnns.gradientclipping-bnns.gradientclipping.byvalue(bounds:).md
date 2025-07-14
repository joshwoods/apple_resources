

- Accelerate
- BNNS
- BNNS.GradientClipping
-  BNNS.GradientClipping.byValue(bounds:) 

Case

# BNNS.GradientClipping.byValue(bounds:)

A constant that indicates that the operation clips gradients to a specified range.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case byValue(bounds: ClosedRange)
```

## Parameters 

`bounds`  

The minimum and maximum clipping values.

## See Also

### Gradient Clipping Functions

case none

A constant that indicates that the operation doesn’t clip gradients.

case byNorm(threshold: Float)

A constant that indicates that the operation clips gradients to a specified Euclidean norm.

case byGlobalNorm(threshold: Float, globalNorm: Float)

A constant that indicates that the operation clips gradients to a specified global Euclidean norm.

