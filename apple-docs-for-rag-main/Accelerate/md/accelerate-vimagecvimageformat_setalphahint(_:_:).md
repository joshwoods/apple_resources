

- Accelerate
-  vImageCVImageFormat_SetAlphaHint(\_:\_:) 

Function

# vImageCVImageFormat_SetAlphaHint(\_:\_:)

Sets the alpha hint of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_SetAlphaHint(
    _ format: vImageCVImageFormat,
    _ alphaIsOne: Int32
) -> vImage_Error
```

## Parameters 

`format`  

The Core Video image format to update.

`alphaIsOne`  

The new value of the alpha hint.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

When an image format contains an alpha channel, but the image is fully opaque, set this property to a nonzero value.

## See Also

### Related Documentation

var alphaIsOpaqueHint: Bool

The alpha hint of the Core Video image format.

### Querying and setting the alpha hint

func vImageCVImageFormat_GetAlphaHint(vImageConstCVImageFormat) -> Int32

Returns the alpha hint of a Core Video image format.

