

- Accelerate
-  vImageOverwriteChannelsWithPixel_ARGB16U(\_:\_:\_:\_:\_:) 

Function

# vImageOverwriteChannelsWithPixel_ARGB16U(\_:\_:\_:\_:\_:)

Overwrites the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageOverwriteChannelsWithPixel_ARGB16U(
    _ the_pixel: UnsafePointer!,
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ copyMask: UInt8,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`the_pixel`  

The source pixel value that provides the new channel values.

`src`  

The source vImage buffer that provides the original pixel values.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`copyMask`  

A bitmask that specifies the channel or channels that the function overwrites with the corresponding channel in the `the_pixel` parameter. The value `0x8` represents channel `0`, the value `0x4` represents channel `1`, the value `0x2` represents channel `2`, and the value `0x2` represents channel `3`.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The following code overwrites channel `0` of the source pixels in `pixelBuffer` with channel `0` of the source pixel value:

```
let pixelBuffer = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40,
                  50, 60, 70, 80],
    size: .init(width: 1, height: 2))

let pixel: [Pixel_16U] =  [101, 102, 103, 104]

pixelBuffer.withUnsafePointerToVImageBuffer { buf in
    _ = vImageOverwriteChannelsWithPixel_ARGB16U(pixel,
                                                 buf,
                                                 buf,
                                                 0x8,
                                                 vImage_Flags(kvImageNoFlags))
}

// Prints:
//      "[101, 20, 30, 40,
//        101, 60, 70, 80]"
print(pixelBuffer.array)
```

## See Also

### Overwriting with pixel values

func vImageOverwriteChannelsWithPixel_ARGB8888(UnsafePointer&lt;UInt8>!, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

func vImageOverwriteChannelsWithPixel_ARGBFFFF(UnsafePointer&lt;Float>!, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer with the specified channels of a pixel value.

