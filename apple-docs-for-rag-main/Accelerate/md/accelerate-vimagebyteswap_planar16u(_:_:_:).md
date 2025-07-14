

- Accelerate
-  vImageByteSwap_Planar16U(\_:\_:\_:) 

Function

# vImageByteSwap_Planar16U(\_:\_:\_:)

Byte-swaps an unsigned 16-bit planar buffer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageByteSwap_Planar16U(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

Call this function to swap the byte ordering of each pixel in an unsigned 16-bit planar image. Byte-swapping converts the image between big endian and little endian architectures.

The following code converts the two pixels in the pixel buffer from `[”AABB”, “11FF”]` to `[”BBAA”, “FF11”]`:

```
let pixelBuffer = vImage.PixelBuffer(
    pixelValues: [
        UInt16("AABB", radix: 16) ?? 0,
        UInt16("11FF", radix: 16) ?? 0],
    size: .init(width: 2, height: 1))

pixelBuffer.withUnsafePointerToVImageBuffer { buf in
    _ = vImageByteSwap_Planar16U(buf,
                                 buf,
                                 vImage_Flags(kvImageNoFlags))
}

// Prints "["bbaa", "ff11"]".
print(pixelBuffer.array.map {String($0, radix: 16)})
```

