

- Accelerate
- vDSP
-  convolve(\_:rowCount:columnCount:with5x5Kernel:result:) 

Type Method

# convolve(\_:rowCount:columnCount:with5x5Kernel:result:)

Calculates the 2D convolution of a double-precision vector with a 5 x 5 kernel.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func convolve(
    _ vector: T,
    rowCount: Int,
    columnCount: Int,
    with5x5Kernel kernel: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Double, U.Element == Double, V.Element == Double
```

## See Also

### Fixed-Size Kernel

static func convolve&lt;T, U>(T, rowCount: Int, columnCount: Int, with3x3Kernel: U) -> [Double]

Returns the 2D convolution of a double-precision vector with a 3 x 3 kernel.

static func convolve&lt;T, U>(T, rowCount: Int, columnCount: Int, with3x3Kernel: U) -> [Float]

Returns the 2D convolution of a single-precision vector with a 3 x 3 kernel.

static func convolve&lt;T, U, V>(T, rowCount: Int, columnCount: Int, with3x3Kernel: U, result: inout V)

Calculates the 2D convolution of a double-precision vector with a 3 x 3 kernel.

static func convolve&lt;T, U, V>(T, rowCount: Int, columnCount: Int, with3x3Kernel: U, result: inout V)

Calculates the 2D convolution of a single-precision vector with a 3 x 3 kernel.

static func convolve&lt;T, U>(T, rowCount: Int, columnCount: Int, with5x5Kernel: U) -> [Double]

Returns the 2D convolution of a double-precision vector with a 5 x 5 kernel.

static func convolve&lt;T, U>(T, rowCount: Int, columnCount: Int, with5x5Kernel: U) -> [Float]

Returns the 2D convolution of a single-precision vector with a 5 x 5 kernel.

static func convolve&lt;T, U, V>(T, rowCount: Int, columnCount: Int, with5x5Kernel: U, result: inout V)

Calculates the 2D convolution of a single-precision vector with a 5 x 5 kernel.

