

- Video Toolbox
-  kVTCompressionPropertyKey_PreserveAlphaChannel 

Global Variable

# kVTCompressionPropertyKey_PreserveAlphaChannel

A key that specifies whether to encode the alpha channel of input video frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_PreserveAlphaChannel: CFString
```

## Discussion

Set this property to false in cases where you’re not interested in preserving alpha, or if you know the alpha channel to be fully opaque.

This property isn’t supported by all encoders.

## See Also

### Bitstream Configuration

let kVTCompressionPropertyKey_Depth: CFString

The pixel depth of the encoded video.

let kVTCompressionPropertyKey_H264EntropyMode: CFString

The entropy encoding mode for H.264 compression.

let kVTCompressionPropertyKey_HDRMetadataInsertionMode: CFString

let kVTCompressionPropertyKey_OutputBitDepth: CFString

let kVTCompressionPropertyKey_ProfileLevel: CFString

The profile and level for the encoded bitstream.

