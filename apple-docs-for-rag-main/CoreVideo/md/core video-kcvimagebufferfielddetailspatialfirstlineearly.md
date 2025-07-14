

- Core Video
-  kCVImageBufferFieldDetailSpatialFirstLineEarly 

Global Variable

# kCVImageBufferFieldDetailSpatialFirstLineEarly

A key to the spatial first line early detail field of the image buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCVImageBufferFieldDetailSpatialFirstLineEarly: CFString
```

## Discussion

The spatial first line early detail field value is of type CFString. The image buffer contains interleaved fields. The first line of image data corresponds to the first top, odd-numbered, field.

## See Also

### Constants

let kCVImageBufferFieldDetailTemporalTopFirst: CFString

A key to the temporal top first detail field of the image buffer.

let kCVImageBufferFieldDetailTemporalBottomFirst: CFString

A key to the temporal bottom first detail field of the image buffer.

let kCVImageBufferFieldDetailSpatialFirstLineLate: CFString

A key to the spatial first line late detail field of the image buffer.

