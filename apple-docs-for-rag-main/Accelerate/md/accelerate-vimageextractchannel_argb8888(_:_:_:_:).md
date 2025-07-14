

- Accelerate
-  vImageExtractChannel_ARGB8888(\_:\_:\_:\_:) 

Function

# vImageExtractChannel_ARGB8888(\_:\_:\_:\_:)

Extracts a single channel from an 8-bit-per-channel, 4-channel interleaved buffer and writes the result to an 8-bit planar buffer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageExtractChannel_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ channelIndex: Int,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the height, width, and rowBytes fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`channelIndex`  

The index of the channel that the function extracts.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The following code extracts channel `1` from the source buffer and writes the result to the destination buffer:

```
let source = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40,
                  50, 60, 70, 80],
    size: .init(width: 1, height: 2))

let destination = vImage.PixelBuffer(
    size: source.size
)

source.withUnsafePointerToVImageBuffer { src in
    destination.withUnsafePointerToVImageBuffer { dst in
        _ = vImageExtractChannel_ARGB8888(src,
                                          dst,
                                          1,
                                          vImage_Flags(kvImageNoFlags))
    }
}

// Prints:
//      "[20,
//        60]"
print(destination.array)
```

## See Also

### Extracting channels

func vImageExtractChannel_ARGB16U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int, vImage_Flags) -> vImage_Error

Extracts a single channel from an unsigned 16-bit-per-channel, 4-channel interleaved buffer and writes the result to an unsigned 16-bit planar buffer.

func vImageExtractChannel_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, Int, vImage_Flags) -> vImage_Error

Extracts a single channel from a 32-bit-per-channel, 4-channel interleaved buffer and writes the result to a 32-bit planar buffer.

