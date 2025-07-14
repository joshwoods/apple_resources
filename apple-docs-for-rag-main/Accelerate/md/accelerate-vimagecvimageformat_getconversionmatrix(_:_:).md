

- Accelerate
-  vImageCVImageFormat_GetConversionMatrix(\_:\_:) 

Function

# vImageCVImageFormat_GetConversionMatrix(\_:\_:)

Returns a pointer to the RGB-to-YpCbCr conversion matrix of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetConversionMatrix(
    _ format: vImageConstCVImageFormat,
    _ outType: UnsafeMutablePointer!
) -> UnsafeRawPointer!
```

## Parameters 

`format`  

The Core Video image format to query.

`outType`  

A pointer to a `vImageMatrixType`.

## Return Value

A pointer to the conversion matrix.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetConversionMatrix(_:_:):

```
let conversionMatrixPointer = withUnsafeBytes(of: cvImageFormat) { bytes in
    var outType = UInt32()

    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetConversionMatrix(format, &outType)
}
```

## See Also

### Querying and setting the conversion matrix

func vImageCVImageFormat_CopyConversionMatrix(vImageCVImageFormat, UnsafeRawPointer, vImageMatrixType) -> vImage_Error

Copies an RGB-to-YpCbCr conversion matrix to an image format’s internal matrix.

