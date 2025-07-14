

- Accelerate
-  vImageCVImageFormat_GetAlphaHint(\_:) 

Function

# vImageCVImageFormat_GetAlphaHint(\_:)

Returns the alpha hint of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetAlphaHint(_ format: vImageConstCVImageFormat) -> Int32
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

Zero if the alpha hint isn’t opaque, or if the hint isn’t set. Nonzero if the alpha hint is fully opaque, even if the encoded values for alpha in the image aren’t `1.0`.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetAlphaHint(_:):

```
let alphaHint = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetAlphaHint(format)
}
```

## See Also

### Related Documentation

var alphaIsOpaqueHint: Bool

The alpha hint of the Core Video image format.

### Querying and setting the alpha hint

func vImageCVImageFormat_SetAlphaHint(vImageCVImageFormat, Int32) -> vImage_Error

Sets the alpha hint of a Core Video image format.

