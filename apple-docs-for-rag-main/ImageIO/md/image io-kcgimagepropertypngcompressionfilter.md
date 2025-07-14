

- Image I/O
-  kCGImagePropertyPNGCompressionFilter 

Global Variable

# kCGImagePropertyPNGCompressionFilter

The PNG filter to apply prior to compression.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCGImagePropertyPNGCompressionFilter: CFString
```

## Discussion

The value of this key is a CFNumber. The number contains a bitwise-OR of one or more filter constants, such as IMAGEIO_PNG_FILTER_AVG or IMAGEIO_PNG_FILTER_SUB. The value has no effect on formats other than PNG.

## See Also

### Pre-Compression Filters

var IMAGEIO_PNG_NO_FILTERS: Int32

No PNG filters.

var IMAGEIO_PNG_FILTER_NONE: Int32

A filter in which each byte is unchanged.

var IMAGEIO_PNG_FILTER_SUB: Int32

A filter in which each byte is replaced with the difference between it and the corresponding byte to its left.

var IMAGEIO_PNG_FILTER_UP: Int32

A filter in which each byte is replaced with the difference between it and the byte above it.

var IMAGEIO_PNG_FILTER_AVG: Int32

A filter in which each byte is replaced with the difference between it and the average of the bytes above it and to its left.

var IMAGEIO_PNG_FILTER_PAETH: Int32

A filter in which each byte is replaced with the difference between it and the Paeth predictor of the bytes to its left, above, and upper left.

