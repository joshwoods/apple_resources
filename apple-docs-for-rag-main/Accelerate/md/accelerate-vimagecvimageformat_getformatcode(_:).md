

- Accelerate
-  vImageCVImageFormat_GetFormatCode(\_:) 

Function

# vImageCVImageFormat_GetFormatCode(\_:)

Returns the four-character code that encodes the pixel format of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetFormatCode(_ format: vImageConstCVImageFormat) -> UInt32
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

The four-character code of the image format, such as kCVPixelFormatType_420YpCbCr8Planar.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetFormatCode(_:):

```
let formatCode = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetFormatCode(format)
}
```

## See Also

### Related Documentation

var formatCode: UInt32

The four-character code that encodes the pixel format of the Core Video image format.

