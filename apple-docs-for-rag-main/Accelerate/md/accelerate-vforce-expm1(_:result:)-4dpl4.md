

- Accelerate
- vForce
-  expm1(\_:result:) 

Type Method

# expm1(\_:result:)

Calculates the *eˣ-1* for each element in a vector of double-precision values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func expm1(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## See Also

### Array-Oriented Exponential and Logarithmic Functions

static func exp&lt;U>(U) -> [Double]

Returns the *e*, raised to the power of each element in a vector of double-precision values.

static func exp&lt;U>(U) -> [Float]

Returns the *e*, raised to the power of each element in a vector of single-precision values.

static func exp&lt;U, V>(U, result: inout V)

Calculates the *e*, raised to the power of each element in a vector of double-precision values.

static func exp&lt;U, V>(U, result: inout V)

Calculates the *e*, raised to the power of each element in a vector of single-precision values.

static func exp2&lt;U>(U) -> [Double]

Returns the 2, raised to the power of each element in a vector of double-precision values.

static func exp2&lt;U>(U) -> [Float]

Returns the 2, raised to the power of each element in a vector of single-precision values.

static func exp2&lt;U, V>(U, result: inout V)

Calculates the 2, raised to the power of each element in a vector of double-precision values.

static func exp2&lt;U, V>(U, result: inout V)

Calculates the 2, raised to the power of each element in a vector of single-precision values.

static func expm1&lt;U>(U) -> [Double]

Returns the *eˣ-1* for each element in a vector of double-precision values.

static func expm1&lt;U>(U) -> [Float]

Returns the *eˣ-1* for each element in a vector of single-precision values.

static func expm1&lt;U, V>(U, result: inout V)

Calculates the *eˣ-1* for each element in a vector of single-precision values.

static func log10&lt;U>(U) -> [Double]

Returns the base 10 logarithm of each element in a vector of double-precision values.

static func log&lt;U>(U) -> [Double]

Returns the natural logarithm for each element in a vector of double-precision values.

static func log&lt;U>(U) -> [Float]

Returns the natural logarithm for each element in a vector of single-precision values.

static func log&lt;U, V>(U, result: inout V)

Calculates the natural logarithm for each element in a vector of double-precision values.

