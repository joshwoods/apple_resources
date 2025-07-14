

- Accelerate
-  vImageAffineWarp_Planar16F(\_:\_:\_:\_:\_:\_:) 

Function

# vImageAffineWarp_Planar16F(\_:\_:\_:\_:\_:\_:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func vImageAffineWarp_Planar16F(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ tempBuffer: UnsafeMutableRawPointer!,
    _ transform: UnsafePointer,
    _ backColor: Pixel_16F,
    _ flags: vImage_Flags
) -> vImage_Error
```

## See Also

### Single-Precision Affine Transformation

func vImageAffineWarp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, Pixel_8, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an 8-bit planar image.

func vImageAffineWarp_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, Pixel_F, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a 32-bit planar image.

func vImageAffineWarp_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an unsigned 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;Int16>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a signed 16-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to an 8-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Applies a single-precision affine transformation to a 32-bit-per-channel, 4-channel interleaved image.

func vImageAffineWarp_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

func vImageAffineWarp_CbCr16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, UnsafePointer&lt;vImage_AffineTransform>, UnsafePointer&lt;UInt16>!, vImage_Flags) -> vImage_Error

