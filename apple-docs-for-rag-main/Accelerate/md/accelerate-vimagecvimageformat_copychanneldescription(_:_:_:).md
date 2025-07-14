

- Accelerate
-  vImageCVImageFormat_CopyChannelDescription(\_:\_:\_:) 

Function

# vImageCVImageFormat_CopyChannelDescription(\_:\_:\_:)

Copies the channel description for a particular channel type to an image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_CopyChannelDescription(
    _ format: vImageCVImageFormat,
    _ desc: UnsafePointer,
    _ type: vImageBufferTypeCode
) -> vImage_Error
```

## Parameters 

`format`  

The vImageCVImageFormat to copy the channel description into.

`desc`  

A pointer to a new vImageChannelDescription to use for the channel type.

`type`  

The type of the channel that you want to set information about, for example, kvImageBufferTypeCode_Luminance.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

## See Also

### Querying and setting channel information

func vImageCVImageFormat_GetChannelCount(vImageConstCVImageFormat) -> UInt32

Returns the number of channels, including alpha, for the Core Video image format.

func vImageCVImageFormat_GetChannelDescription(vImageConstCVImageFormat, vImageBufferTypeCode) -> UnsafePointer&lt;vImageChannelDescription>!

Returns the channel description for a particular channel type.

func vImageCVImageFormat_GetChannelNames(vImageConstCVImageFormat) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns the names of the channels of a Core Video image format.

struct vImageChannelDescription

A description of the range and clamp limits for a pixel format.

