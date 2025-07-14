

- Accelerate
- vDSP
-  subtract(\_:from:count:result:) 

Type Method

# subtract(\_:from:count:result:)

Calculates the single-precision elementwise subtraction of a complex vector from a complex vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func subtract(
    _ splitComplexB: DSPSplitComplex,
    from splitComplexA: DSPSplitComplex,
    count: Int,
    result: inout DSPSplitComplex
)
```

## See Also

### Subtraction

static func subtract&lt;T, U>(U, T) -> [Double]

Returns the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U>(U, T) -> [Float]

Returns the single-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the single-precision element-wise subtraction of two vectors.

static func subtract(DSPDoubleSplitComplex, from: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise subtraction of a complex vector from a complex vector.

static func subtract&lt;T, U>(multiplication: (a: U, b: Double), T) -> [Double]

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Double]

Returns the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U>(multiplication: (a: U, b: Float), T) -> [Float]

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Float]

Returns the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Double), T, result: inout V)

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Float), T, result: inout V)

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Double]

Returns the double-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Float]

Returns the single-precision element-wise difference of the products of two pairs of vectors.

