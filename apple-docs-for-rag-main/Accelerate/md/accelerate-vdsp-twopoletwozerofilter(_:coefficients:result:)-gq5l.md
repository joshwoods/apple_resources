

- Accelerate
- vDSP
-  twoPoleTwoZeroFilter(\_:coefficients:result:) 

Type Method

# twoPoleTwoZeroFilter(\_:coefficients:result:)

Performs single-precision, two-pole, two-zero recursive filtering.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func twoPoleTwoZeroFilter(
    _ source: U,
    coefficients: (Float, Float, Float, Float, Float),
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## See Also

### Vector-to-Vector Recursive Filtering on Real Vectors

static func twoPoleTwoZeroFilter&lt;U>(U, coefficients: (Double, Double, Double, Double, Double)) -> [Double]

Returns the result of double-precision, two-pole, two-zero recursive filtering.

static func twoPoleTwoZeroFilter&lt;U>(U, coefficients: (Float, Float, Float, Float, Float)) -> [Float]

Returns the result of single-precision, two-pole, two-zero recursive filtering.

static func twoPoleTwoZeroFilter&lt;U, V>(U, coefficients: (Double, Double, Double, Double, Double), result: inout V)

Performs double-precision, two-pole, two-zero recursive filtering.

