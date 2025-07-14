

- Video Toolbox
-  kVTCompressionPropertyKey_MVHEVCViewIDs 

Global Variable

# kVTCompressionPropertyKey_MVHEVCViewIDs

The identifiers of the views corresponding to the video layers in a multiview encoding operation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
let kVTCompressionPropertyKey_MVHEVCViewIDs: CFString
```

## Discussion

This property is specific to MV-HEVC.

The entries in the specified array should be in the same order and have the same count as the value specified in kVTCompressionPropertyKey_MVHEVCVideoLayerIDs.

The default value is `NULL`.

## See Also

### Multiview compression

let kVTCompressionPropertyKey_MVHEVCVideoLayerIDs: CFString

The identifiers of the video layers to encode in a multiview encoding operation.

let kVTCompressionPropertyKey_MVHEVCLeftAndRightViewIDs: CFString

Specifies which view identifier corresponds to the left eye and right eye.

