

- Accelerate
-  vImageFlatten_RGBA16U(\_:\_:\_:\_:\_:) 

Function

# vImageFlatten_RGBA16U(\_:\_:\_:\_:\_:)

Performs an alpha composite of an unsigned 16-bit-per-channel, 4-channel RGBA buffer over a solid background color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageFlatten_RGBA16U(
    _ rgbaSrc: UnsafePointer,
    _ rgbaDst: UnsafePointer,
    _ rgbaBackgroundColorPtr: UnsafePointer,
    _ isImagePremultiplied: Bool,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`rgbaSrc`  

The source vImage buffer.

`rgbaDst`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`rgbaBackgroundColorPtr`  

A pixel value that defines the solid background color.

`isImagePremultiplied`  

A Boolean value that specifes whether the source image has premultiplied alpha.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to flatten the source image:

```
 resultAlpha = (pixelAlpha * 65535 + (65535 - pixelAlpha) * backgroundAlpha + 32767) / 65535

 if(isImagePremultiplied)
     resultColor = (pixelColor * 65535 + (65535 - pixelAlpha) * backgroundColor + 32767) / 65535
 else
     resultColor = (pixelColor * pixelAlpha + (65535 - pixelAlpha) * backgroundColor + 32767) / 65535
```

## See Also

### Flattening 4-channel,16-bit images

func vImageFlatten_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of an unsigned 16-bit-per-channel, 4-channel ARGB buffer over a solid background color.

func vImageFlatten_RGBA16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a fixed-point 16-bit-per-channel, 4-channel RGBA buffer over a solid background color.

func vImageFlatten_ARGB16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a fixed-point 16-bit-per-channel, 4-channel ARGB buffer over a solid background color.

