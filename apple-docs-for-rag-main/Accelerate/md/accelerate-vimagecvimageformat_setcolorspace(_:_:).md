

- Accelerate
-  vImageCVImageFormat_SetColorSpace(\_:\_:) 

Function

# vImageCVImageFormat_SetColorSpace(\_:\_:)

Sets the color space of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_SetColorSpace(
    _ format: vImageCVImageFormat,
    _ colorspace: CGColorSpace!
) -> vImage_Error
```

## Parameters 

`format`  

The Core Video image format to update.

`colorspace`  

The new color space for the format.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

For RGB, indexed, and grayscale images, the color space of a Core Video image format describes the image encoding.

For YpCbCr images, the color space describes the image encoding of the RGB image that’s the result of unapplying the RGB-to-YpCbCr conversion matrix.

## See Also

### Related Documentation

var colorSpace: CGColorSpace?

The color space of the Core Video image format.

### Querying and setting the color space

func vImageCVImageFormat_GetColorSpace(vImageConstCVImageFormat) -> Unmanaged&lt;CGColorSpace>!

Returns the color space of a Core Video image format.

