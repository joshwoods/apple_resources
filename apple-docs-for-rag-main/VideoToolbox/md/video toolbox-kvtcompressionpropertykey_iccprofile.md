

- Video Toolbox
-  kVTCompressionPropertyKey_ICCProfile 

Global Variable

# kVTCompressionPropertyKey_ICCProfile

The ICC profile for compressed content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_ICCProfile: CFString
```

## Discussion

If the video encoder enforces specific colorimetry, this property will be read-only (VTSessionSetProperty(_:key:value:) will return kVTPropertyReadOnlyErr). If this property and any of the other color properties (color primaries, transfer function, or YCbCr matrix) are set, they should be set to consistent values, or undefined behavior may occur. The value will be set on the format description for output sample buffers. `NULL` can be a valid value for this property.

## See Also

### Color

let kVTCompressionPropertyKey_AlphaChannelMode: CFString

let kVTCompressionPropertyKey_ColorPrimaries: CFString

The color primaries for compressed content.

let kVTCompressionPropertyKey_ContentLightLevelInfo: CFString

let kVTCompressionPropertyKey_GammaLevel: CFString

let kVTCompressionPropertyKey_MasteringDisplayColorVolume: CFString

let kVTCompressionPropertyKey_TransferFunction: CFString

The transfer function for compressed content.

let kVTCompressionPropertyKey_YCbCrMatrix: CFString

The YCbCr matrix for compressed content.

