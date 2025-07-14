

- Accelerate
- vImage_Buffer
-  init(cgImage:flags:) 

Initializer

# init(cgImage:flags:)

Creates a new buffer with the contents of a Core Graphics image.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
init(
    cgImage: CGImage,
    flags options: vImage.Options = .noFlags
) throws
```

## Parameters 

`cgImage`  

The source image.

`options`  

The options to use when performing the operation.

## Discussion

This function initializes a vImage buffer using the format of the Core Graphics image.

## See Also

### Consuming and producing Core Graphics images

init(cgImage: CGImage, format: vImage_CGImageFormat, flags: vImage.Options) throws

Creates a new buffer with the contents of a Core Graphics image using the supplied image format.

func createCGImage(format: vImage_CGImageFormat, flags: vImage.Options) throws -> CGImage

Creates a Core Graphics image from the vImage buffer.

