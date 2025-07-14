

- Video Toolbox
-  kVTCompressionPropertyKey_TransferFunction 

Global Variable

# kVTCompressionPropertyKey_TransferFunction

The transfer function for compressed content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_TransferFunction: CFString
```

## Discussion

If the video encoder enforces specific colorimetry, this property will be read-only (VTSessionSetProperty(_:key:value:) will return kVTPropertyReadOnlyErr). The value is set on the format description for output sample buffers.

## See Also

### Color

let kVTCompressionPropertyKey_AlphaChannelMode: CFString

let kVTCompressionPropertyKey_ColorPrimaries: CFString

The color primaries for compressed content.

let kVTCompressionPropertyKey_ContentLightLevelInfo: CFString

let kVTCompressionPropertyKey_GammaLevel: CFString

let kVTCompressionPropertyKey_ICCProfile: CFString

The ICC profile for compressed content.

let kVTCompressionPropertyKey_MasteringDisplayColorVolume: CFString

let kVTCompressionPropertyKey_YCbCrMatrix: CFString

The YCbCr matrix for compressed content.

