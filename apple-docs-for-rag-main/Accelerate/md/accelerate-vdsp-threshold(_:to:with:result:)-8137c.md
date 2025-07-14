

- Accelerate
- vDSP
-  threshold(\_:to:with:result:) 

Type Method

# threshold(\_:to:with:result:)

Calculates the elements of the supplied single-precision vector after applying a specified thresholding rule.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func threshold(
    _ vector: U,
    to lowerBound: Float,
    with rule: vDSP.ThresholdRule,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Threshold Operations

static func threshold&lt;U>(U, to: Double, with: vDSP.ThresholdRule&lt;Double>) -> [Double]

Returns the elements of the supplied double-precision vector after applying a specified thresholding rule.

static func threshold&lt;U>(U, to: Float, with: vDSP.ThresholdRule&lt;Float>) -> [Float]

Returns the elements of the supplied single-precision vector after applying a specified thresholding rule.

static func threshold&lt;U, V>(U, to: Double, with: vDSP.ThresholdRule&lt;Double>, result: inout V)

Calculates the elements of the supplied double-precision vector after applying a specified thresholding rule.

enum ThresholdRule

Constants that specify vector threshold rules.

