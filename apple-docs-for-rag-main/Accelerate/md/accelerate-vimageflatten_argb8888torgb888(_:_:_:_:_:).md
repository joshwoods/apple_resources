

- Accelerate
-  vImageFlatten_ARGB8888ToRGB888(\_:\_:\_:\_:\_:) 

Function

# vImageFlatten_ARGB8888ToRGB888(\_:\_:\_:\_:\_:)

Flattens an 8-bit-per-channel ARGB buffer against a solid background to produce an 8-bit-per-channel RGB result.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageFlatten_ARGB8888ToRGB888(
    _: UnsafePointer,
    _: UnsafePointer,
    _: UnsafePointer,
    _: Bool,
    _: vImage_Flags
) -> vImage_Error
```

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

### Parameters

argb8888Src  
The source vImage buffer.

rgb888dest  
A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

backgroundColor  
A pixel value that defines the solid background color.

isImagePremultiplied  
A Boolean value that specifes whether the source image has premultiplied alpha.

flags  
The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

The function uses the following calculation to flatten the source image:

```
 if( isImagePremultiplied )
     color = (color * 255 + (255 - alpha) * backgroundColor + 127) / 255
 else
     color = (color * alpha + (255 - alpha) * backgroundColor + 127) / 255
```

## See Also

### Flattening 4-channel, 8-bit images to three channels

func vImageFlatten_BGRA8888ToRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Flattens an 8-bit-per-channel BGRA buffer against a solid background to produce an 8-bit-per-channel RGB result.

func vImageFlatten_RGBA8888ToRGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, Bool, vImage_Flags) -> vImage_Error

Flattens an 8-bit-per-channel RGBA buffer against a solid background to produce an 8-bit-per-channel RGB result.

