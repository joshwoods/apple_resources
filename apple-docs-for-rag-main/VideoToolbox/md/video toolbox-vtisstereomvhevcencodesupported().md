

- Video Toolbox
-  VTIsStereoMVHEVCEncodeSupported() 

Function

# VTIsStereoMVHEVCEncodeSupported()

Returns a Boolean value that indicates whether the system supports MV-HEVC encoding.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func VTIsStereoMVHEVCEncodeSupported() -> Bool
```

## Return Value

true if the system supports MV-HEVC encoding; otherwise, false.

## Discussion

A return value of true doesn’t guarantee that encoding resources are available at all times.

## See Also

### Encoding Multi-Image Frames

func VTCompressionSessionEncodeMultiImageFrame(VTCompressionSession, taggedBuffers: [CMTaggedBuffer], presentationTimeStamp: CMTime, duration: CMTime, frameProperties: CFDictionary?, infoFlagsOut: UnsafeMutablePointer&lt;VTEncodeInfoFlags>?, outputHandler: VTCompressionOutputHandler) -> OSStatus

Passes a multi-image frame to a compression session for encoding and provides a callback to handle the output.

