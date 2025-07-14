

- Accelerate
-  vImageCVImageFormat_GetChannelDescription(\_:\_:) 

Function

# vImageCVImageFormat_GetChannelDescription(\_:\_:)

Returns the channel description for a particular channel type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetChannelDescription(
    _ format: vImageConstCVImageFormat,
    _ type: vImageBufferTypeCode
) -> UnsafePointer!
```

## Parameters 

`format`  

The Core Video image format to query.

`type`  

The type of the channel that you want information about. For example, kvImageBufferTypeCode_Luminance.

## Return Value

A pointer to a vImageChannelDescription structure that contains the channel description.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetChannelDescription(_:_:):

```
let channelDescription = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetChannelDescription(format,
                                                     vImageBufferTypeCode(kvImageBufferTypeCode_Luminance))
}
```

## See Also

### Related Documentation

func channelDescription(bufferType: vImage.BufferType) -> vImageChannelDescription?

Returns the range and clamp limits for a specified channel in a Core Video image format.

### Querying and setting channel information

func vImageCVImageFormat_GetChannelCount(vImageConstCVImageFormat) -> UInt32

Returns the number of channels, including alpha, for the Core Video image format.

func vImageCVImageFormat_CopyChannelDescription(vImageCVImageFormat, UnsafePointer&lt;vImageChannelDescription>, vImageBufferTypeCode) -> vImage_Error

Copies the channel description for a particular channel type to an image format.

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

struct vImageChannelDescription

A description of the range and clamp limits for a pixel format.

