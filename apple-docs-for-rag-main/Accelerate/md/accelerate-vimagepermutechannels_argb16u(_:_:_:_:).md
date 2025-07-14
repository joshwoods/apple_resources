

- Accelerate
-  vImagePermuteChannels_ARGB16U(\_:\_:\_:\_:) 

Function

# vImagePermuteChannels_ARGB16U(\_:\_:\_:\_:)

Permutes the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePermuteChannels_ARGB16U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ permuteMap: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`permuteMap`  

An array of four 8-bit integers with the values `0`, `1`, `2`, and 3, in some order. Each value specifies the channel from the source image that the function copies to the destination channel at the corresponding index.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The following code reverses the channel ordering of a pixel buffer:

```
let pixelBuffer = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40],
    size: .init(width: 1, height: 1))

pixelBuffer.withUnsafePointerToVImageBuffer { buf in
    _ = vImagePermuteChannels_ARGB16U(buf,
                                       buf,
                                       [3, 2, 1, 0],
                                       vImage_Flags(kvImageNoFlags))
}

// Prints "[40, 30, 20, 10]".
print(pixelBuffer.array)
```

## See Also

### Permuting channels

func vImagePermuteChannels_RGB888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>!, vImage_Flags) -> vImage_Error

Permutes the channels of an 8-bit-per-channel, 3-channel interleaved buffer.

func vImagePermuteChannels_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of an 8-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannels_ARGB16F(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of a floating-point 16-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannels_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, vImage_Flags) -> vImage_Error

Permutes the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

