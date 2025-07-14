

- Accelerate
- vDSP
-  downsample(\_:decimationFactor:filter:) 

Type Method

# downsample(\_:decimationFactor:filter:)

Returns the downsampled double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func downsample(
    _ source: U,
    decimationFactor: Int,
    filter: T
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Mentioned in 

Resampling a signal with decimation

## See Also

### Real Vectors

Resampling a signal with decimation

Reduce the sample rate of a signal by specifying a decimation factor and applying a custom antialiasing filter.

static func downsample&lt;T, U>(U, decimationFactor: Int, filter: T) -> [Float]

Returns the downsampled single-precision vector.

static func downsample&lt;T, U, V>(U, decimationFactor: Int, filter: T, result: inout V)

Calculates the downsampled double-precision vector.

static func downsample&lt;T, U, V>(U, decimationFactor: Int, filter: T, result: inout V)

Calculates the downsampled single-precision vector.

