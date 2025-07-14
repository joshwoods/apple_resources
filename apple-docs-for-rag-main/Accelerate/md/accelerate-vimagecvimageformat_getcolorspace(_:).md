

- Accelerate
-  vImageCVImageFormat_GetColorSpace(\_:) 

Function

# vImageCVImageFormat_GetColorSpace(\_:)

Returns the color space of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetColorSpace(_ format: vImageConstCVImageFormat) -> Unmanaged!
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

The color space of the specified image format.

## Discussion

For RGB, indexed, and grayscale images, the color space of a Core Video image format describes the image encoding.

For YpCbCr images, the color space describes the image encoding of the RGB image that’s the result of unapplying the RGB-to-YpCbCr conversion matrix.

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetColorSpace(_:):

```
let colorSpace = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetColorSpace(format)
}
```

## See Also

### Related Documentation

var colorSpace: CGColorSpace?

The color space of the Core Video image format.

### Querying and setting the color space

func vImageCVImageFormat_SetColorSpace(vImageCVImageFormat, CGColorSpace!) -> vImage_Error

Sets the color space of a Core Video image format.

