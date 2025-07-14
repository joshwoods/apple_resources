

- Core Video
-  kCVImageBufferChromaSubsampling_422 

Global Variable

# kCVImageBufferChromaSubsampling_422

A key that indicates the original chroma-subsampled data used 4:2:2 formatting.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCVImageBufferChromaSubsampling_422: CFString
```

## Discussion

Each pixel has a `Y` value, and `U` and `V` values are shared horizontally between 2 neighboring pixels.

## See Also

### Constants

let kCVImageBufferChromaSubsampling_420: CFString

A key that indicates the original chroma-subsampled data used 4:2:0 formatting.

let kCVImageBufferChromaSubsampling_411: CFString

A key that indicates the original chroma-subsampled data used 4:1:1 formatting.

