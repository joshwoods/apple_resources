

- Video Toolbox
-  VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:outputCallback:decompressionSessionOut:) 

Function

# VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:outputCallback:decompressionSessionOut:)

Creates a session for decompressing video frames.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTDecompressionSessionCreate(
    allocator: CFAllocator?,
    formatDescription videoFormatDescription: CMVideoFormatDescription,
    decoderSpecification videoDecoderSpecification: CFDictionary?,
    imageBufferAttributes destinationImageBufferAttributes: CFDictionary?,
    outputCallback: UnsafePointer?,
    decompressionSessionOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`allocator`  

An allocator for the session. Pass `NULL` to use the default allocator.

`videoFormatDescription`  

The description of the source video frames.

`videoDecoderSpecification`  

The particular video decoder that must be used. Pass `NULL` to let VideoToolbox choose a decoder.

`destinationImageBufferAttributes`  

Requirements for the emitted pixel buffers. Pass `NULL` to set no requirements.

`outputCallback`  

The callback to be called with decompressed frames. Pass `NULL` only if you’ll be calling VTDecompressionSessionDecodeFrame(_:sampleBuffer:flags:infoFlagsOut:outputHandler:) for decoding frames.

`decompressionSessionOut`  

A pointer to a variable to receive the new decompression session.

## Discussion

Decompressed frames are emitted through calls to `outputCallback`.

## See Also

### Creating a Session

func VTDecompressionSessionCreate(allocator: CFAllocator?, formatDescription: CMVideoFormatDescription, decoderSpecification: CFDictionary?, imageBufferAttributes: CFDictionary?, decompressionSessionOut: UnsafeMutablePointer&lt;VTDecompressionSession?>) -> OSStatus

