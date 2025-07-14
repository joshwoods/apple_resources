

- Video Toolbox
-  kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata 

Global Variable

# kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata

A key that indicates to generate per frame HDR Metadata and attach it to the resulting decoded pixel buffers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
let kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata: CFString
```

## Discussion

If the color space and YCbCr matrix match a supported HDR format such as HLG (kCMFormatDescriptionTransferFunction_ITU_R_2100_HLG) the system analyzes the decoded frame and adds the metadata as an attachment to the pixel buffers.

## See Also

### Post-Decompression Processing

let kVTDecompressionPropertyKey_PixelTransferProperties: CFString

Specific pixel transfer features to be used during decompression.

let kVTVideoDecoderSpecification_RequiredDecoderGPURegistryID: CFString

let kVTVideoDecoderSpecification_PreferredDecoderGPURegistryID: CFString

let kVTDecompressionPropertyKey_UsingGPURegistryID: CFString

let kVTDecompressionPropertyKey_PropagatePerFrameHDRDisplayMetadata: CFString

let kVTDecompressionPropertyKey_DecoderProducesRAWOutput: CFString

let kVTDecompressionPropertyKey_RequestRAWOutput: CFString

