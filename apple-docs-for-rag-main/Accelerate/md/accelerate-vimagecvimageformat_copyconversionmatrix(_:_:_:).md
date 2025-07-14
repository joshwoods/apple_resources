

- Accelerate
-  vImageCVImageFormat_CopyConversionMatrix(\_:\_:\_:) 

Function

# vImageCVImageFormat_CopyConversionMatrix(\_:\_:\_:)

Copies an RGB-to-YpCbCr conversion matrix to an image format’s internal matrix.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_CopyConversionMatrix(
    _ format: vImageCVImageFormat,
    _ matrix: UnsafeRawPointer,
    _ inType: vImageMatrixType
) -> vImage_Error
```

## Parameters 

`format`  

The destination vImageCVImageFormat instance.

`matrix`  

The matrix that the function copies to the destination image format.

`inType`  

The type of the matrix.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

## See Also

### Querying and setting the conversion matrix

func vImageCVImageFormat_GetConversionMatrix(vImageConstCVImageFormat, UnsafeMutablePointer&lt;vImageMatrixType>!) -> UnsafeRawPointer!

Returns a pointer to the RGB-to-YpCbCr conversion matrix of a Core Video image format.

