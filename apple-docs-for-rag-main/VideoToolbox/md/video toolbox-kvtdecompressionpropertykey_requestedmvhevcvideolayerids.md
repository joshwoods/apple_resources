

- Video Toolbox
-  kVTDecompressionPropertyKey_RequestedMVHEVCVideoLayerIDs 

Global Variable

# kVTDecompressionPropertyKey_RequestedMVHEVCVideoLayerIDs

Requests multi-image decoding of specific MV-HEVC video layers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_RequestedMVHEVCVideoLayerIDs: CFString
```

## Discussion

This property is specific to MV-HEVC. The use of it requires you to use the VTDecompressionSessionSetMultiImageCallback function to install a callback capable of receiving CMTaggedBufferGroupRef objects in response to multi-image frame decode requests.

MV-HEVC video layer IDs not in this list don’t need to be output, and the decoder may skip decoding them if not otherwise necessary.

The property is NULL by default. If this property is NULL, MV-HEVC ignores layers other than the base layer.

Note

In multiview decompression, a single video sample contains a single frame (with one PTS) that the system decodes to produce multiple images.

