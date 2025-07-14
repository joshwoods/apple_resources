

- Accelerate
- BNNS
- BNNS.GradientClipping
-  BNNS.GradientClipping.none 

Case

# BNNS.GradientClipping.none

A constant that indicates that the operation doesn’t clip gradients.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case none
```

## See Also

### Gradient Clipping Functions

case byValue(bounds: ClosedRange&lt;Float>)

A constant that indicates that the operation clips gradients to a specified range.

case byNorm(threshold: Float)

A constant that indicates that the operation clips gradients to a specified Euclidean norm.

case byGlobalNorm(threshold: Float, globalNorm: Float)

A constant that indicates that the operation clips gradients to a specified global Euclidean norm.

