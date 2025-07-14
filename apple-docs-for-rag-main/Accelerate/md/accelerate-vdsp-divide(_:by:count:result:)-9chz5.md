

- Accelerate
- vDSP
-  divide(\_:by:count:result:) 

Type Method

# divide(\_:by:count:result:)

Calculates the single-precision elementwise division of a complex vector by a complex vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func divide(
    _ splitComplexA: DSPSplitComplex,
    by splitComplexB: DSPSplitComplex,
    count: Int,
    result: inout DSPSplitComplex
)
```

## See Also

### Division

static func divide&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Double) -> [Double]

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise division of two vectors.

static func divide&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Float) -> [Float]

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise division of two vectors.

static func divide&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(U, Double, result: inout V)

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;U, V>(U, Float, result: inout V)

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise division of two vectors.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise division of two vectors.

static func divide(DSPDoubleSplitComplex, by: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

static func divide&lt;U>(DSPSplitComplex, by: U, result: inout DSPSplitComplex)

Calculates the single-precision elementwise division of a complex vector by a real vector.

static func divide&lt;U>(DSPDoubleSplitComplex, by: U, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

