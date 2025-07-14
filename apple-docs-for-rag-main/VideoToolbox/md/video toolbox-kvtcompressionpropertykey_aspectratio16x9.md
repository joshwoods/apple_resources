

- Video Toolbox
-  kVTCompressionPropertyKey_AspectRatio16x9 

Global Variable

# kVTCompressionPropertyKey_AspectRatio16x9

A Boolean value indicating whether the DV video stream should have the 16x9 flag set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_AspectRatio16x9: CFString
```

## Discussion

This property is supported by the DV25/50 family of encoders.

When false, the picture aspect ratio is 4:3. When true, the picture aspect ratio is 16:9. Either way, a fixed aspect ratio is used (the specific value depends on whether the format is NTSC or PAL).

## See Also

### Clean Aperture and Pixel Aspect Ratio

let kVTCompressionPropertyKey_CleanAperture: CFString

The clean aperture for encoded frames.

let kVTCompressionPropertyKey_FieldCount: CFString

The field count indicating whether the frames should be encoded progressive (1) or interlaced (2).

let kVTCompressionPropertyKey_FieldDetail: CFString

Field ordering for encoded interlaced frames.

let kVTCompressionPropertyKey_PixelAspectRatio: CFString

The pixel aspect ratio for encoded frames.

let kVTCompressionPropertyKey_ProgressiveScan: CFString

A Boolean value indicating whether the DV video stream should have the progressive flag set.

