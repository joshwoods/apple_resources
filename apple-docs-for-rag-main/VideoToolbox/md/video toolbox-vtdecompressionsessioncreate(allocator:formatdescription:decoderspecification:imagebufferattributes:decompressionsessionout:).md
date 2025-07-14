

- Video Toolbox
-  VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:decompressionSessionOut:) 

Function

# VTDecompressionSessionCreate(allocator:formatDescription:decoderSpecification:imageBufferAttributes:decompressionSessionOut:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func VTDecompressionSessionCreate(
    allocator: CFAllocator?,
    formatDescription videoFormatDescription: CMVideoFormatDescription,
    decoderSpecification videoDecoderSpecification: CFDictionary?,
    imageBufferAttributes destinationImageBufferAttributes: CFDictionary?,
    decompressionSessionOut: UnsafeMutablePointer
) -> OSStatus
```

## See Also

### Creating a Session

func VTDecompressionSessionCreate(allocator: CFAllocator?, formatDescription: CMVideoFormatDescription, decoderSpecification: CFDictionary?, imageBufferAttributes: CFDictionary?, outputCallback: UnsafePointer&lt;VTDecompressionOutputCallbackRecord>?, decompressionSessionOut: UnsafeMutablePointer&lt;VTDecompressionSession?>) -> OSStatus

Creates a session for decompressing video frames.

