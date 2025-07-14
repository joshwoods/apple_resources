

- Video Toolbox
-  kVTCompressionPropertyKey_ProgressiveScan 

Global Variable

# kVTCompressionPropertyKey_ProgressiveScan

A Boolean value indicating whether the DV video stream should have the progressive flag set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_ProgressiveScan: CFString
```

## Discussion

This property is supported by the DV25/50 family of encoders. If false, content is encoded as interlaced. If true, content is encoded as progressive. The value of this property fixes the kVTCompressionPropertyKey_FieldCount and kVTCompressionPropertyKey_FieldDetail properties.

## See Also

### Clean Aperture and Pixel Aspect Ratio

let kVTCompressionPropertyKey_AspectRatio16x9: CFString

A Boolean value indicating whether the DV video stream should have the 16x9 flag set.

let kVTCompressionPropertyKey_CleanAperture: CFString

The clean aperture for encoded frames.

let kVTCompressionPropertyKey_FieldCount: CFString

The field count indicating whether the frames should be encoded progressive (1) or interlaced (2).

let kVTCompressionPropertyKey_FieldDetail: CFString

Field ordering for encoded interlaced frames.

let kVTCompressionPropertyKey_PixelAspectRatio: CFString

The pixel aspect ratio for encoded frames.

