

- Core Video
-  kCVImageBufferFieldDetailTemporalTopFirst 

Global Variable

# kCVImageBufferFieldDetailTemporalTopFirst

A key to the temporal top first detail field of the image buffer.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCVImageBufferFieldDetailTemporalTopFirst: CFString
```

## Discussion

The temporal top first detail field value is of type CFString. The image buffer contains complete fields in alternating order. The top, odd-numbered, fields contain image data captured at an earlier time than bottom, even-numbered, fields.

## See Also

### Constants

let kCVImageBufferFieldDetailTemporalBottomFirst: CFString

A key to the temporal bottom first detail field of the image buffer.

let kCVImageBufferFieldDetailSpatialFirstLineEarly: CFString

A key to the spatial first line early detail field of the image buffer.

let kCVImageBufferFieldDetailSpatialFirstLineLate: CFString

A key to the spatial first line late detail field of the image buffer.

