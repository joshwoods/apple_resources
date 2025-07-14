

- Video Toolbox
-  VTIsStereoMVHEVCDecodeSupported() 

Function

# VTIsStereoMVHEVCDecodeSupported()

Returns a Boolean value that indicates whether the system supports MV-HEVC decoding.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func VTIsStereoMVHEVCDecodeSupported() -> Bool
```

## Return Value

true if the system supports MV-HEVC decoding; otherwise, false.

## Discussion

A return value of true doesn’t guarantee that decoding resources are available at all times.

## See Also

### Decoding Multi-Image Frames

typealias VTDecompressionMultiImageCapableOutputHandler

A type alias for callback that the system invokes when it finishes decompressing a frame.

