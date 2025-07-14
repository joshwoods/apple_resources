

- Video Toolbox
-  kVTDecompressionPropertyKey_DecoderProducesRAWOutput 

Global Variable

# kVTDecompressionPropertyKey_DecoderProducesRAWOutput

macOS 15.0+

``` source
let kVTDecompressionPropertyKey_DecoderProducesRAWOutput: CFString
```

## Discussion

```
@constant       kVTDecompressionPropertyKey_DecoderProducesRAWOutput
@abstract
   Indicates whether the decoder can produce RAW output requiring a VTRAWProcessingSession for post-decode processing.
@discussion
   If this property is not implemented, it is assumed that the decoder does not produce RAW output.
   If the decoder reports that it produces RAW output the VTDecompressionSession will internally invoke a VTRAWProcessingSession by default to produce
   processed output.
   If the client sets kVTDecompressionPropertyKey_RequestRAWOutput, the VTDecompressionSession will do no processing and return the decoder's native RAW
   output, and any requested destinationImageBufferAttributes on the VTDecompressionSession will be ignored.
```

## See Also

### Post-Decompression Processing

let kVTDecompressionPropertyKey_PixelTransferProperties: CFString

Specific pixel transfer features to be used during decompression.

let kVTVideoDecoderSpecification_RequiredDecoderGPURegistryID: CFString

let kVTVideoDecoderSpecification_PreferredDecoderGPURegistryID: CFString

let kVTDecompressionPropertyKey_UsingGPURegistryID: CFString

let kVTDecompressionPropertyKey_PropagatePerFrameHDRDisplayMetadata: CFString

let kVTDecompressionPropertyKey_GeneratePerFrameHDRDisplayMetadata: CFString

A key that indicates to generate per frame HDR Metadata and attach it to the resulting decoded pixel buffers.

let kVTDecompressionPropertyKey_RequestRAWOutput: CFString

