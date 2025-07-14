

- Image I/O
-  IMAGEIO_PNG_FILTER_UP 

Global Variable

# IMAGEIO_PNG_FILTER_UP

A filter in which each byte is replaced with the difference between it and the byte above it.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var IMAGEIO_PNG_FILTER_UP: Int32 { get }
```

## See Also

### Pre-Compression Filters

let kCGImagePropertyPNGCompressionFilter: CFString

The PNG filter to apply prior to compression.

var IMAGEIO_PNG_NO_FILTERS: Int32

No PNG filters.

var IMAGEIO_PNG_FILTER_NONE: Int32

A filter in which each byte is unchanged.

var IMAGEIO_PNG_FILTER_SUB: Int32

A filter in which each byte is replaced with the difference between it and the corresponding byte to its left.

var IMAGEIO_PNG_FILTER_AVG: Int32

A filter in which each byte is replaced with the difference between it and the average of the bytes above it and to its left.

var IMAGEIO_PNG_FILTER_PAETH: Int32

A filter in which each byte is replaced with the difference between it and the Paeth predictor of the bytes to its left, above, and upper left.

