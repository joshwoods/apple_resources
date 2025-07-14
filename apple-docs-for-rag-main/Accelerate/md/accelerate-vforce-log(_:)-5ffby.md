

- Accelerate
- vForce
-  log(\_:) 

Type Method

# log(\_:)

Returns the natural logarithm for each element in a vector of single-precision values.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func log(_ vector: U) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`vector`  

The input vector.

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

Calculates the *eˣ-1* for each element in a vector of double-precision values.

static func expm1&lt;U, V>(U, result: inout V)

Calculates the *eˣ-1* for each element in a vector of single-precision values.

static func log10&lt;U>(U) -> [Double]

Returns the base 10 logarithm of each element in a vector of double-precision values.

static func log&lt;U>(U) -> [Double]

Returns the natural logarithm for each element in a vector of double-precision values.

static func log&lt;U, V>(U, result: inout V)

Calculates the natural logarithm for each element in a vector of double-precision values.

