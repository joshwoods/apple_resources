

- Accelerate
-  vImagePermuteChannelsWithMaskedInsert_ARGB8888(\_:\_:\_:\_:\_:\_:) 

Function

# vImagePermuteChannelsWithMaskedInsert_ARGB8888(\_:\_:\_:\_:\_:\_:)

Permutes and overwrites the channels of an 8-bit-per-channel, 4-channel interleaved buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePermuteChannelsWithMaskedInsert_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ permuteMap: UnsafePointer,
    _ copyMask: UInt8,
    _ backgroundColor: UnsafePointer,
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

`copyMask`  

A bitmask that specifies the channel or channels that the function overwrites with the corresponding channel in the `backgroundColor` parameter. The value `0x8` represents channel `0`, the value `0x4` represents channel `1`, the value `0x2` represents channel `2`, and the value `0x2` represents channel `3`.

`backgroundColor`  

The 8-bit-per-channel ARGB value that the function writes to the destination based on the `copyMask` value.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This fused operation provides the same functionality as vImagePermuteChannels_ARGB8888(_:_:_:_:) followed by vImageOverwriteChannelsWithScalar_ARGB8888(_:_:_:_:_:) but offers higher performance than calling the two functions separately.

The following code reverses the channel ordering of a pixel buffer and overwrites channel `0` of the destination with element `0` of the background color:

```
let pixelBuffer = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40],
    size: .init(width: 1, height: 1))

let backgroundColor: [Pixel_8] = [101, 102, 103, 104]

pixelBuffer.withUnsafePointerToVImageBuffer { buf in
    _ = vImagePermuteChannelsWithMaskedInsert_ARGB8888(buf,
                                                       buf,
                                                       [3, 2, 1, 0],
                                                       0x8,
                                                       backgroundColor,
                                                       vImage_Flags(kvImageNoFlags))
}

// Prints "[101, 30, 20, 10]".
print(pixelBuffer.array)
```

## See Also

### Permuting channels with masked insert

func vImagePermuteChannelsWithMaskedInsert_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;UInt16>, vImage_Flags) -> vImage_Error

Permutes and overwrites the channels of an unsigned 16-bit-per-channel, 4-channel interleaved buffer.

func vImagePermuteChannelsWithMaskedInsert_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt8>, UInt8, UnsafePointer&lt;Float>, vImage_Flags) -> vImage_Error

Permutes and overwrites the channels of a floating-point 32-bit-per-channel, 4-channel interleaved buffer.

