

- Accelerate
-  vImageCVImageFormat_GetChannelNames(\_:) 

Function

# vImageCVImageFormat_GetChannelNames(\_:)

Returns the names of the channels of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetChannelNames(_ format: vImageConstCVImageFormat) -> UnsafePointer!
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

A pointer to an array that contains the vImageBufferTypeCode elements that correspond to the names of the channels in the image.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetChannelNames(_:):

```
let channelNames = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetChannelNames(format)
}
```

## See Also

### Related Documentation

var channels: [vImage.BufferType]

The channels of the Core Video image format.

### Querying and setting channel information

func vImageCVImageFormat_GetChannelCount(vImageConstCVImageFormat) -> UInt32

Returns the number of channels, including alpha, for the Core Video image format.

func vImageCVImageFormat_GetChannelDescription(vImageConstCVImageFormat, vImageBufferTypeCode) -> UnsafePointer&lt;vImageChannelDescription>!

Returns the channel description for a particular channel type.

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

struct vImageChannelDescription

A description of the range and clamp limits for a pixel format.

