

- Video Toolbox
-  kVTDecompressionPropertyKey_PixelTransferProperties 

Global Variable

# kVTDecompressionPropertyKey_PixelTransferProperties

Specific pixel transfer features to be used during decompression.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_PixelTransferProperties: CFString
```

## Discussion

This property value is a doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum object containing properties from `VTPixelTransferProperties.h`.

## See Also

### Post-Decompression Processing

let kVTVideoDecoderSpecification_RequiredDecoderGPURegistryID: CFString

let kVTVideoDecoderSpecification_PreferredDecoderGPURegistryID: CFString

let kVTDecompressionPropertyKey_UsingGPURegistryID: CFString

let kVTDecompressionPropertyKey_PropagatePerFrameHDRDisplayMetadata: CFString

let kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata: CFString

A key that indicates to generate per frame HDR Metadata and attach it to the resulting decoded pixel buffers.

let kVTDecompressionPropertyKey_DecoderProducesRAWOutput: CFString

let kVTDecompressionPropertyKey_RequestRAWOutput: CFString

