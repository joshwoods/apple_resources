

- Accelerate
- vImage
- vImage.PixelBuffer
-  vImage.PixelBuffer.Histogram8888 

Type Alias

# vImage.PixelBuffer.Histogram8888

The histogram for four channel 8-bit pixel buffers.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
typealias Histogram8888 = ([vImagePixelCount], [vImagePixelCount], [vImagePixelCount], [vImagePixelCount])
```

Available when `Format` conforms to `PixelFormat` and `Format.ComponentType` is `UInt8`.

## See Also

### Type aliases

typealias Histogram888

The histogram for three channel 8-bit pixel buffers.

typealias HistogramFFF

The histogram for three channel 32-bit pixel buffers.

typealias HistogramFFFF

The histogram for four channel 32-bit pixel buffers.

