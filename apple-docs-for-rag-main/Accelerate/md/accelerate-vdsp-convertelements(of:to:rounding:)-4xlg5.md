

- Accelerate
- vDSP
-  convertElements(of:to:rounding:) 

Type Method

# convertElements(of:to:rounding:)

Converts double-precision values to 16-bit signed integers.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convertElements(
    of source: U,
    to destination: inout V,
    rounding: vDSP.RoundingMode
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Int16
```

## Parameters 

`source`  

The source vector.

`destination`  

On output, the source values converted to integer values.

`rounding`  

The rounding mode.

## See Also

### Type Methods

static func absolute&lt;U>(U) -> [Double]

Returns the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U>(U) -> [Float]

Returns the absolute value of each element in the supplied single-precision vector.

static func absolute&lt;V>(DSPSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied single-precision complex vector.

static func absolute&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied double-precision complex vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied single-precision vector.

static func add&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise sum of two vectors.

static func add&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise sum of two vectors.

static func add&lt;U, V>(Double, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise sum of two vectors.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise sum of two vectors.

static func add(DSPSplitComplex, to: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise sum of the supplied complex vectors.

