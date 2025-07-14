

- Accelerate
- BNNS
- BNNS.GradientClipping
-  BNNS.GradientClipping.byNorm(threshold:) 

Case

# BNNS.GradientClipping.byNorm(threshold:)

A constant that indicates that the operation clips gradients to a specified Euclidean norm.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case byNorm(threshold: Float)
```

## Parameters 

`threshold`  

The maximum Euclidean norm.

## See Also

### Gradient Clipping Functions

case none

A constant that indicates that the operation doesn’t clip gradients.

case byValue(bounds: ClosedRange&lt;Float>)

A constant that indicates that the operation clips gradients to a specified range.

case byGlobalNorm(threshold: Float, globalNorm: Float)

A constant that indicates that the operation clips gradients to a specified global Euclidean norm.

