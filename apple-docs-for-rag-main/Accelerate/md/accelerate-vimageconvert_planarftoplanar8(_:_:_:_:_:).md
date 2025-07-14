

- Accelerate
-  vImageConvert_PlanarFtoPlanar8(\_:\_:\_:\_:\_:) 

Function

# vImageConvert_PlanarFtoPlanar8(\_:\_:\_:\_:\_:)

Converts a floating-point 32-bit planar buffer to an 8-bit planar buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.3+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConvert_PlanarFtoPlanar8(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ maxFloat: Pixel_F,
    _ minFloat: Pixel_F,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`maxFloat`  

The maximum source pixel value.

`minFloat`  

The minimum source pixel value.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The function uses the following calculation to perform the conversion:

```
uint8_t result = SATURATED_CLIP_0_to_255( 255.0f * ( srcPixel - minFloat ) / (maxFloat - minFloat) + 0.5f );
```

## See Also

### Converting from floating-point 32-bit-per-channel buffers

func vImageConvert_PlanarFtoPlanar8_dithered(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Pixel_F, Pixel_F, Int32, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to an 8-bit planar buffer using the specified dithering algorithm.

func vImageConvert_FTo16S(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to a signed 16-bit planar buffer.

func vImageConvert_FTo16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Float, Float, vImage_Flags) -> vImage_Error

Converts a floating-point 32-bit planar buffer to an unsigned 16-bit planar buffer.

