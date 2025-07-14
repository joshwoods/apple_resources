

- Accelerate
- vForce
-  cosh(\_:result:) 

Type Method

# cosh(\_:result:)

Calculates the hyperbolic cosine of each element in a vector of single-precision values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func cosh(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Array-Oriented Hyperbolic Functions

static func acosh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic cosine of each element in a vector of double-precision values.

static func acosh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic cosine of each element in a vector of single-precision values.

static func acosh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic cosine of each element in a vector of double-precision values.

static func acosh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic cosine of each element in a vector of single-precision values.

static func asinh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic sine of each element in a vector of double-precision values.

static func asinh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic sine of each element in a vector of single-precision values.

static func asinh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic sine of each element in a vector of double-precision values.

static func asinh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic sine of each element in a vector of single-precision values.

static func atanh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic tangent of each element in a vector of double-precision values.

static func atanh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic tangent of each element in a vector of single-precision values.

static func atanh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic tangent of each element in a vector of double-precision values.

static func atanh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic tangent of each element in a vector of single-precision values.

static func cosh&lt;U>(U) -> [Double]

Returns the hyperbolic cosine of each element in a vector of double-precision values.

static func cosh&lt;U>(U) -> [Float]

Returns the hyperbolic cosine of each element in a vector of single-precision values.

static func cosh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic cosine of each element in a vector of double-precision values.

