

- Accelerate
- vDSP
-  convolve(\_:withKernel:) 

Type Method

# convolve(\_:withKernel:)

Returns the 1D convolution of a double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convolve(
    _ vector: T,
    withKernel kernel: U
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Parameters 

`vector`  

The input signal vector.

`kernel`  

The filter vector.

## Return Value

The convolution result.

## See Also

### Real Vectors

static func convolve&lt;T, U>(T, withKernel: U) -> [Float]

Returns the 1D convolution of a single-precision vector.

static func convolve&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the 1D convolution of a double-precision vector.

static func convolve&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the 1D convolution of a single-precision vector.

static func correlate&lt;T, U>(T, withKernel: U) -> [Double]

Returns the correlation of a double-precision signal vector and a filter vector.

static func correlate&lt;T, U>(T, withKernel: U) -> [Float]

Returns the correlation of a single-precision signal vector and a filter vector.

static func correlate&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the correlation of a double-precision signal vector and a filter vector.

static func correlate&lt;T, U, V>(T, withKernel: U, result: inout V)

Calculates the correlation of a single-precision signal vector and a filter vector.

