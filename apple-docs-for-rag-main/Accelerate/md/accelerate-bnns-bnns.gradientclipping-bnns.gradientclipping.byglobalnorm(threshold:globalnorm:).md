

- Accelerate
- BNNS
- BNNS.GradientClipping
-  BNNS.GradientClipping.byGlobalNorm(threshold:globalNorm:) 

Case

# BNNS.GradientClipping.byGlobalNorm(threshold:globalNorm:)

A constant that indicates that the operation clips gradients to a specified global Euclidean norm.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
case byGlobalNorm(
    threshold: Float,
    globalNorm: Float = 0
)
```

## Parameters 

`threshold`  

The maximum Euclidean norm.

`globalNorm`  

An optional value for a known global Euclidean norm. Set to `0` to specify that the function computes the norm.

## See Also

### Gradient Clipping Functions

case none

A constant that indicates that the operation doesn’t clip gradients.

case byValue(bounds: ClosedRange&lt;Float>)

A constant that indicates that the operation clips gradients to a specified range.

case byNorm(threshold: Float)

A constant that indicates that the operation clips gradients to a specified Euclidean norm.

