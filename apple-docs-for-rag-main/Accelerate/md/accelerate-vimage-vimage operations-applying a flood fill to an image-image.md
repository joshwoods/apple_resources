

- Accelerate
- vImage
- vImage Operations
-  Applying a flood fill to an image 

API Collection

# Applying a flood fill to an image

Fill connected components of an image with a new color.

## Topics

### Flood-filling buffers

Applying flood fills to an image

Fill consistently colored connected parts of an image with a new color.

func vImageFloodFill_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, Pixel_8, Int32, vImage_Flags) -> vImage_Error

Applies a flood-fill operation to an 8-bit planar image.

func vImageFloodFill_Planar16U(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, Pixel_16U, Int32, vImage_Flags) -> vImage_Error

Applies a flood fill-operation to an unsigned 16-bit planar image.

func vImageFloodFill_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafeMutablePointer&lt;UInt8>!, Int32, vImage_Flags) -> vImage_Error

Applies a flood-fill operation to an 8-bit-per-channel, four-channel interleaved image.

func vImageFloodFill_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImagePixelCount, vImagePixelCount, UnsafeMutablePointer&lt;UInt16>!, Int32, vImage_Flags) -> vImage_Error

Applies a flood-fill operation to an unsigned 16-bit-per-channel, four-channel interleaved image.

## See Also

### Applying color transforms to images

Transforming with lookup tables

Use lookup tables to apply color transformations to images.

Transforming with polynomials

Use polynomials to apply color transformations to images.

Transforming with matrix multiplication

Use matrix multiplication to apply color transformations to images.

Transforming with a gamma function

Use gamma functions to apply color transformations to images.

