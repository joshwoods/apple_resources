

- Accelerate
-  vImageOverwriteChannelsWithScalar_ARGBFFFF(\_:\_:\_:\_:\_:) 

Function

# vImageOverwriteChannelsWithScalar_ARGBFFFF(\_:\_:\_:\_:\_:)

Overwrites the selected channels of a 32-bit-per-channel, 4-channel interleaved buffer with the specified scalar value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageOverwriteChannelsWithScalar_ARGBFFFF(
    _ scalar: Pixel_F,
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ copyMask: UInt8,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`scalar`  

The scalar value that provides the new channel values.

`src`  

The source vImage buffer that provides the original pixel values.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`copyMask`  

A bitmask that specifies the channel or channels that the function overwrites with the scalar value. The value `0x8` represents channel `0`, the value `0x4` represents channel `1`, the value `0x2` represents channel `2`, and the value `0x2` represents channel `3`.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The following code overwrites channel `0` of the source pixels in `pixelBuffer` with the scalar value:

```
let pixelBuffer = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40,
                  50, 60, 70, 80],
    size: .init(width: 1, height: 2))

let scalar: Pixel_F = 101

pixelBuffer.withUnsafePointerToVImageBuffer { buf in
    _ = vImageOverwriteChannelsWithScalar_ARGBFFFF(scalar,
                                                   buf,
                                                   buf,
                                                   0x8,
                                                   vImage_Flags(kvImageNoFlags))
}

// Prints:
//      "[101.0, 20.0, 30.0, 40.0,
//        101.0, 60.0, 70.0, 80.0]"
print(pixelBuffer.array)
```

## See Also

### Overwriting with scalar values

func vImageOverwriteChannelsWithScalar_Planar8(Pixel_8, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites an 8-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16U(Pixel_16U, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites an unsigned 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16S(Pixel_16S, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a signed 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_Planar16F(Pixel_16F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a floating-point 16-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_PlanarF(Pixel_F, UnsafePointer&lt;vImage_Buffer>, vImage_Flags) -> vImage_Error

Overwrites a floating-point 32-bit planar buffer with the specified scalar value in place.

func vImageOverwriteChannelsWithScalar_ARGB8888(Pixel_8, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UInt8, vImage_Flags) -> vImage_Error

Overwrites the selected channels of an 8-bit-per-channel, 4-channel interleaved buffer with the specified scalar value.

