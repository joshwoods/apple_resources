

- Accelerate
-  vImageMatrixMultiply_ARGB8888(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageMatrixMultiply_ARGB8888(\_:\_:\_:\_:\_:\_:\_:)

Multiplies each pixel in an interleaved four-channel, 8-bit source image by a matrix to produce an interleaved four-channel, 8-bit destination image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageMatrixMultiply_ARGB8888(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ matrix: UnsafePointer,
    _ divisor: Int32,
    _ pre_bias: UnsafePointer!,
    _ post_bias: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`matrix`  

An array of values that contains the 4 x 4 matrix elements.

`divisor`  

A value that the function divides the matrix multiplication result by after adding postbias.

`pre_bias`  

An array that contains four bias values. The function adds the corresponding bias value to each source value before the matrix multiplication step. Pass `nil` to specify zero prebias.

`post_bias`  

An array that contains four bias values. The function adds the corresponding bias value to each destination value after the matrix multiplication step. Pass `nil` to specify zero postbias.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Mentioned in 

Applying vImage operations to regions of interest

## Discussion

This function treats the four-channel source and destination pixels as four-element vectors. The operation multiplies each source pixel by the 4 x 4 matrix to produce the destination pixel.

The following code shows a single-pixel image that contains the ARGB value `(10, 20, 30, 40)`. The matrix permutes the channel values to produce a single-pixel destination image that contains the ARGB value `(40, 30, 20, 10)`.

```
let size = vImage.Size(width: 1, height: 1)

let source = vImage.PixelBuffer(
    pixelValues: [10, 20, 30, 40],
    size: size)

let destination = vImage.PixelBuffer(
    size: size)

let matrix: [Int16] = [
    0, 0, 0, 1,
    0, 0, 1, 0,
    0, 1, 0, 0,
    1, 0, 0, 0
]

source.withUnsafePointerToVImageBuffer { src in
    destination.withUnsafePointerToVImageBuffer { dest in

        _ = vImageMatrixMultiply_ARGB8888(
            src,
            dest,
            matrix,
            1,
            nil,
            nil,
            vImage_Flags(kvImageNoFlags))

    }
}

// Prints "[40, 30, 20, 10]".
print(destination.array)
```

## See Also

### Multiplying interleaved pixels by a matrix

func vImageMatrixMultiply_ARGBFFFF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>!, UnsafePointer&lt;Float>!, vImage_Flags) -> vImage_Error

Multiplies each pixel in an interleaved four-channel, 32-bit source image by a matrix to produce an interleaved four-channel, 32-bit destination image.

func vImageMatrixMultiply_ARGB8888ToPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Int16>, Int32, UnsafePointer&lt;Int16>!, Int32, vImage_Flags) -> vImage_Error

Multiplies each pixel in an interleaved four-channel, 8-bit source image by a matrix to produce a planar 8-bit destination image.

func vImageMatrixMultiply_ARGBFFFFToPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>!, Float, vImage_Flags) -> vImage_Error

Multiplies each pixel in an interleaved four-channel, 32-bit source image by a matrix to produce a planar 32-bit destination image.

