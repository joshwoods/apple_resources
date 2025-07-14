

- Accelerate
- vDSP
-  vDSP.ThresholdRule 

Enumeration

# vDSP.ThresholdRule

Constants that specify vector threshold rules.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
enum ThresholdRule where T : BinaryFloatingPoint
```

## Topics

### Threshold rules

case clampToThreshold

Returns the threshold if the input value is less than threshold; otherwise returns the input value.

case signedConstant(T)

Returns the negated constant if the input value is less than the threshold; otherwise returns the constant.

case zeroFill

Returns `0` if the input value is less than the threshold; otherwise returns the input value.

## See Also

### Threshold Operations

static func threshold&lt;U>(U, to: Double, with: vDSP.ThresholdRule&lt;Double>) -> [Double]

Returns the elements of the supplied double-precision vector after applying a specified thresholding rule.

static func threshold&lt;U>(U, to: Float, with: vDSP.ThresholdRule&lt;Float>) -> [Float]

Returns the elements of the supplied single-precision vector after applying a specified thresholding rule.

static func threshold&lt;U, V>(U, to: Double, with: vDSP.ThresholdRule&lt;Double>, result: inout V)

Calculates the elements of the supplied double-precision vector after applying a specified thresholding rule.

static func threshold&lt;U, V>(U, to: Float, with: vDSP.ThresholdRule&lt;Float>, result: inout V)

Calculates the elements of the supplied single-precision vector after applying a specified thresholding rule.

