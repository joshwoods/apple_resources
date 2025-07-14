

- Video Toolbox
-  kVTDecompressionPropertyKey_RequestRAWOutput 

Global Variable

# kVTDecompressionPropertyKey_RequestRAWOutput

macOS 15.0+

``` source
let kVTDecompressionPropertyKey_RequestRAWOutput: CFString
```

## Discussion

```
@constant       kVTDecompressionPropertyKey_RequestRAWOutput
@abstract
   For decoders which produce RAW output, this property requests that the VTDecompressionSession provide output which has not been processed.
@discussion
   When a decoder produces RAW output (signalled by kVTDecompressionPropertyKey_DecoderProducesRAWOutput) the VTDecompressionSession will automatically
   invoke a VTRAWProcessingSession with default settings and emit processed frames by default, or when kVTDecompressionPropertyKey_RequestRAWOutput is set
   to kCFBooleanFalse.
   If a client wants to run a VTRAWProcessingSession on the RAW output themselves in order to control the post-decode processing of the decoded CVPixelBuffers,
   they must set kVTDecompressionPropertyKey_RequestRAWOutput to kCFBooleanTrue.
   If kVTDecompressionPropertyKey_RequestRAWOutput has been enabled and the decoder produces RAW output, the VTDecompressionSession 
   will return CVPixelBuffers in the decoder's native RAW format.  Any destinationImageBufferAttributes set on the VTDecompressionSession will be ignored.
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

let kVTDecompressionPropertyKey_DecoderProducesRAWOutput: CFString

