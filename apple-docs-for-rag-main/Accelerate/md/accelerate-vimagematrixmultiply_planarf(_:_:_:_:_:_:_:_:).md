

- Accelerate
-  vImageMatrixMultiply_PlanarF(\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageMatrixMultiply_PlanarF(\_:\_:\_:\_:\_:\_:\_:\_:)

Multiplies each pixel in a set of 32-bit source image planes by a matrix to produce a set of 32-bit destination image planes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageMatrixMultiply_PlanarF(
    _ srcs: UnsafeMutablePointer?>,
    _ dests: UnsafeMutablePointer?>,
    _ src_planes: UInt32,
    _ dest_planes: UInt32,
    _ matrix: UnsafePointer,
    _ pre_bias: UnsafePointer!,
    _ post_bias: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`srcs`  

A pointer to an array of vImage buffers. Each buffer represents a source plane.

`dests`  

A pointer to an array of vImage buffers. Each buffer represents a destination plane.

`src_planes`  

The number of source planes.

`dest_planes`  

The number of destination planes.

`matrix`  

An array of values that contains the `src_planes` rows multiplied by `dest_planes` columns 2D matrix elements.

`pre_bias`  

An array of bias values for each source plane. The function adds the corresponding bias value to each source value before the matrix multiplication step. Pass `nil` to specify zero prebias.

`post_bias`  

An array of bias values for each source plane. The function adds the corresponding bias value to each destination value after the matrix multiplication step. Pass `nil` to specify zero postbias.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function treats corresponding pixels in the source buffers as `m`-element vectors, and the corresponding pixels in the destination buffers as `n`-element vectors. Therefore, the multiplication requires an `m x n` matrix, that is, a matrix with `src_planes` rows and `dest_planes` columns.

The following code shows three source planes multiplied by a three-element column matrix to produce a single destination plane. The values in the matrix represent the Rec. 709 luminance coefficients that convert the color source pixels to a grayscale destination image. The three source planes represent the individual red, green, and blue channels of an image that contains a red pixel, a green pixel, and a blue pixel.

```
let size = vImage.Size(width: 1, height: 3)

let red = vImage.PixelBuffer(
    pixelValues: [1, 0, 0],
    size: size)
let green = vImage.PixelBuffer(
    pixelValues: [0, 1, 0],
    size: size)
let blue = vImage.PixelBuffer(
    pixelValues: [0, 0, 1],
    size: size)

let destination = vImage.PixelBuffer(
    size: size)

let redCoefficient: Float = 0.2126
let greenCoefficient: Float = 0.7152
let blueCoefficient: Float = 0.0722

let matrix = [
    redCoefficient,
    greenCoefficient,
    blueCoefficient
]

red.withUnsafePointerToVImageBuffer { r in
    green.withUnsafePointerToVImageBuffer { g in
        blue.withUnsafePointerToVImageBuffer { b in
            destination.withUnsafePointerToVImageBuffer { dest in

                var srcs: [UnsafePointer?] = [ r, g, b ]
                var dests: [UnsafePointer?] = [ dest ]

                vImageMatrixMultiply_PlanarF(
                    &srcs,
                    &dests,
                    3,
                    1,
                    matrix,
                    nil,
                    nil,
                    vImage_Flags(kvImageNoFlags))
            }
        }
    }
}

// Prints "[0.2126, 0.7152, 0.0722]".
print(destination.array)
```

On return, the destination buffer contains a grayscale representation of the red, green, and blue source buffers.

## See Also

### Multiplying multiple-plane pixels by a matrix

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

func vImageMatrixMultiply_Planar8(UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UInt32, UInt32, UnsafePointer&lt;Int16>, Int32, UnsafePointer&lt;Int16>!, UnsafePointer&lt;Int32>!, vImage_Flags) -> vImage_Error

Multiplies each pixel in a set of 8-bit source image planes by a matrix to produce a set of 8-bit destination image planes.

func vImageMatrixMultiply_Planar16S(UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UnsafeMutablePointer&lt;UnsafePointer&lt;vImage_Buffer>?>, UInt32, UInt32, UnsafePointer&lt;Int16>, Int32, UnsafePointer&lt;Int16>!, UnsafePointer&lt;Int32>!, vImage_Flags) -> vImage_Error

Multiplies each pixel in a set of 16-bit source image planes by a matrix to produce a set of 8-bit destination image planes.

