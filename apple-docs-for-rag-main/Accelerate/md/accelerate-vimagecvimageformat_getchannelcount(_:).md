

- Accelerate
-  vImageCVImageFormat_GetChannelCount(\_:) 

Function

# vImageCVImageFormat_GetChannelCount(\_:)

Returns the number of channels, including alpha, for the Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetChannelCount(_ format: vImageConstCVImageFormat) -> UInt32
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

The number of channels.

## Discussion

This function returns the number of interleaved or planar channels.

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetChannelCount(_:):

```
let channelCount = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetChannelCount(format)
}
```

## See Also

### Related Documentation

var channelCount: UInt32

The number of channels, including alpha, for the Core Video image format.

### Querying and setting channel information

func vImageCVImageFormat_GetChannelDescription(vImageConstCVImageFormat, vImageBufferTypeCode) -> UnsafePointer&lt;vImageChannelDescription>!

Returns the channel description for a particular channel type.

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

struct vImageChannelDescription

A description of the range and clamp limits for a pixel format.

