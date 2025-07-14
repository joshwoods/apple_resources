

- Accelerate
-  vImageFlatten_RGBAFFFF(\_:\_:\_:\_:\_:) 

Function

# vImageFlatten_RGBAFFFF(\_:\_:\_:\_:\_:)

Performs an alpha composite of a 32-bit-per-channel, 4-channel RGBA buffer over a solid background color.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageFlatten_RGBAFFFF(
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
 resultAlpha = pixelAlpha + (1 - pixelAlpha) * backgroundAlpha

 if(isImagePremultiplied)
     resultColor = pixelColor + (1 - pixelAlpha) * backgroundColor
 else
     resultColor = pixelColor * pixelAlpha + (1 - pixelAlpha) * backgroundColor
```

## See Also

### Flattening 4-channel, 32-bit images

func vImageFlatten_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Bool, vImage_Flags) -> vImage_Error

Performs an alpha composite of a 32-bit-per-channel, 4-channel ARGB buffer over a solid background color.

