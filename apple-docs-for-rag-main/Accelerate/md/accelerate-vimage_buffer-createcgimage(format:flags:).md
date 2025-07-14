

- Accelerate
- vImage_Buffer
-  createCGImage(format:flags:) 

Instance Method

# createCGImage(format:flags:)

Creates a Core Graphics image from the vImage buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func createCGImage(
    format: vImage_CGImageFormat,
    flags options: vImage.Options = .noFlags
) throws -> CGImage
```

## Parameters 

`format`  

The desired format.

`options`  

The options to use when performing the operation.

## Return Value

A Core Graphics image that represents the contents of the vImage buffer.

## Mentioned in 

Creating a Core Graphics Image from a vImage Buffer

## See Also

### Consuming and producing Core Graphics images

init(cgImage: CGImage, flags: vImage.Options) throws

Creates a new buffer with the contents of a Core Graphics image.

init(cgImage: CGImage, format: vImage_CGImageFormat, flags: vImage.Options) throws

Creates a new buffer with the contents of a Core Graphics image using the supplied image format.

