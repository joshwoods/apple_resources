

- Accelerate
- vDSP
-  convolve(\_:rowCount:columnCount:withKernel:kernelRowCount:kernelColumnCount:) 

Type Method

# convolve(\_:rowCount:columnCount:withKernel:kernelRowCount:kernelColumnCount:)

Returns the 2D convolution of a single-precision vector with an arbitrarily sized kernel.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convolve(
    _ vector: T,
    rowCount: Int,
    columnCount: Int,
    withKernel kernel: U,
    kernelRowCount: Int,
    kernelColumnCount: Int
) -> [Float] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Float, U.Element == Float
```

## See Also

### Arbitrary-Size Kernel

static func convolve&lt;T, U>(T, rowCount: Int, columnCount: Int, withKernel: U, kernelRowCount: Int, kernelColumnCount: Int) -> [Double]

Returns the 2D convolution of a double-precision vector with an arbitrarily sized kernel.

static func convolve&lt;T, U, V>(T, rowCount: Int, columnCount: Int, withKernel: U, kernelRowCount: Int, kernelColumnCount: Int, result: inout V)

Calculates the 2D convolution of a double-precision vector with an arbitrarily sized kernel.

static func convolve&lt;T, U, V>(T, rowCount: Int, columnCount: Int, withKernel: U, kernelRowCount: Int, kernelColumnCount: Int, result: inout V)

Calculates the 2D convolution of a single-precision vector with an arbitrarily sized kernel.

