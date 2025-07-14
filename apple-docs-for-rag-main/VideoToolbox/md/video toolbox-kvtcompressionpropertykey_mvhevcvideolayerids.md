

- Video Toolbox
-  kVTCompressionPropertyKey_MVHEVCVideoLayerIDs 

Global Variable

# kVTCompressionPropertyKey_MVHEVCVideoLayerIDs

The identifiers of the video layers to encode in a multiview encoding operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MVHEVCVideoLayerIDs: CFString
```

## Discussion

This property is specific to MV-HEVC.

Specifying layer ID values advises the encoder to expect CMTaggedBufferGroupRef objects with specific CMTag values that reference them.

The default value is `NULL`.

## See Also

### Multiview compression

let kVTCompressionPropertyKey_MVHEVCViewIDs: CFString

The identifiers of the views corresponding to the video layers in a multiview encoding operation.

let kVTCompressionPropertyKey_MVHEVCLeftAndRightViewIDs: CFString

Specifies which view identifier corresponds to the left eye and right eye.

