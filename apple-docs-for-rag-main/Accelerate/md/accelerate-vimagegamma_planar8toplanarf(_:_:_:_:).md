

- Accelerate
-  vImageGamma_Planar8toPlanarF(\_:\_:\_:\_:) 

Function

# vImageGamma_Planar8toPlanarF(\_:\_:\_:\_:)

Applies a gamma function to an 8-bit planar image to produce a 32-bit planar image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageGamma_Planar8toPlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ gamma: GammaFunction!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`gamma`  

The gamma function object.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

This function maps 8-bit values in the range `0...255` to the floating-point range `0.0...1.0`.

```
let source = vImage.PixelBuffer(
    pixelValues: [  1,
                    3,
                    5,
                   15,
                   17,
                   51 ],
    size: vImage.Size(width: 1, height: 6))

let destination = vImage.PixelBuffer(
    size: source.size)

let gamma = vImageCreateGammaFunction(
    1.0,
    Int32(kvImageGamma_UseGammaValue),
    vImage_Flags(kvImageNoFlags))

defer {
    vImageDestroyGammaFunction(gamma)
}

source.withUnsafePointerToVImageBuffer { src in
    destination.withUnsafePointerToVImageBuffer { dest in

        _ = vImageGamma_Planar8toPlanarF(
            src,
            dest,
            gamma,
            vImage_Flags(kvImageNoFlags))

    }
}

// Prints "[1.0, 3.0, 5.0, 15.0, 17.0, 51.0]".
print(destination.array.map { $0 * 255 })
```

## See Also

### Applying a gamma function

func vImageCreateGammaFunction(Float, Int32, vImage_Flags) -> GammaFunction!

Returns a gamma function object.

Gamma function types

Types of full- or half-precision gamma functions.

func vImageGamma_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a 32-bit planar image to produce an 8-bit planar image.

func vImageGamma_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a PlanarF image.

func vImageDestroyGammaFunction(GammaFunction!)

Destroys a gamma function object.

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

