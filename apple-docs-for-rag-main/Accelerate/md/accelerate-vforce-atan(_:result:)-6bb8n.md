

- Accelerate
- vForce
-  atan(\_:result:) 

Type Method

# atan(\_:result:)

Calculates the arctangent of each element in a vector of single-precision values.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func atan(
    _ vector: U,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Array-Oriented Trigonometric Functions

static func acos&lt;U>(U) -> [Double]

Returns the arccosine of each element in a vector of double-precision values.

static func acos&lt;U>(U) -> [Float]

Returns the arccosine of each element in a vector of single-precision values.

static func acos&lt;U, V>(U, result: inout V)

Calculates the arccosine of each element in a vector of double-precision values.

static func acos&lt;U, V>(U, result: inout V)

Calculates the arccosine of each element in a vector of single-precision values.

static func asin&lt;U>(U) -> [Double]

Returns the arcsine of each element in a vector of double-precision values.

static func asin&lt;U>(U) -> [Float]

Returns the arcsine of each element in a vector of single-precision values.

static func asin&lt;U, V>(U, result: inout V)

Calculates the arcsine of each element in a vector of double-precision values.

static func asin&lt;U, V>(U, result: inout V)

Calculates the arcsine of each element in a vector of single-precision values.

static func atan&lt;U>(U) -> [Double]

Returns the arctangent of each element in a vector of double-precision values.

static func atan&lt;U>(U) -> [Float]

Returns the arctangent of each element in a vector of single-precision values.

static func atan&lt;U, V>(U, result: inout V)

Calculates the arctangent of each element in a vector of double-precision values.

static func atan2&lt;U, V>(x: U, y: V) -> [Double]

Returns the arctangent of each pair of elements in two vectors of double-precision values.

static func atan2&lt;U, V>(x: U, y: V) -> [Float]

Returns the arctangent of each pair of elements in two vectors of single-precision values.

static func atan2&lt;T, U, V>(x: T, y: U, result: inout V)

Calculates the arctangent of each pair of elements in two vectors of double-precision values.

static func atan2&lt;T, U, V>(x: T, y: U, result: inout V)

Calculates the arctangent of each pair of elements in two vectors of single-precision values.

