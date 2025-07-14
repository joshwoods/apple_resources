

- Video Toolbox
-  kVTCompressionPropertyKey_Depth 

Global Variable

# kVTCompressionPropertyKey_Depth

The pixel depth of the encoded video.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_Depth: CFString
```

## Discussion

This property is only supported by video encoders for formats that are tied to particular pixel formats (for example, 16-bit RGB, 24-bit RGB).

## See Also

### Bitstream Configuration

let kVTCompressionPropertyKey_PreserveAlphaChannel: CFString

A key that specifies whether to encode the alpha channel of input video frames.

let kVTCompressionPropertyKey_H264EntropyMode: CFString

The entropy encoding mode for H.264 compression.

let kVTCompressionPropertyKey_HDRMetadataInsertionMode: CFString

let kVTCompressionPropertyKey_OutputBitDepth: CFString

let kVTCompressionPropertyKey_ProfileLevel: CFString

The profile and level for the encoded bitstream.

