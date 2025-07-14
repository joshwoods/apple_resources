

- Accelerate
- vDSP
-  threshold(\_:to:with:) 

Type Method

# threshold(\_:to:with:)

Returns the elements of the supplied double-precision vector after applying a specified thresholding rule.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func threshold(
    _ vector: U,
    to lowerBound: Double,
    with rule: vDSP.ThresholdRule
) -> [Double] where U : AccelerateBuffer, U.Element == Double
```

## See Also

### Threshold Operations

static func threshold&lt;U>(U, to: Float, with: vDSP.ThresholdRule&lt;Float>) -> [Float]

Returns the elements of the supplied single-precision vector after applying a specified thresholding rule.

static func threshold&lt;U, V>(U, to: Double, with: vDSP.ThresholdRule&lt;Double>, result: inout V)

Calculates the elements of the supplied double-precision vector after applying a specified thresholding rule.

static func threshold&lt;U, V>(U, to: Float, with: vDSP.ThresholdRule&lt;Float>, result: inout V)

Calculates the elements of the supplied single-precision vector after applying a specified thresholding rule.

enum ThresholdRule

Constants that specify vector threshold rules.

