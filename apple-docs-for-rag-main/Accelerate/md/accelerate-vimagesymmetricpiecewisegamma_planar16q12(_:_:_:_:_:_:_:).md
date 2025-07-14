

- Accelerate
-  vImageSymmetricPiecewiseGamma_Planar16Q12(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImageSymmetricPiecewiseGamma_Planar16Q12(\_:\_:\_:\_:\_:\_:\_:)

Applies a symmetric piecewise gamma function to transform a 16Q12 planar image to an 8-bit planar image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func vImageSymmetricPiecewiseGamma_Planar16Q12(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ exponentialCoeffs: UnsafePointer,
    _ gamma: Float,
    _ linearCoeffs: UnsafePointer,
    _ boundary: Pixel_16S,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`exponentialCoeffs`  

An array of three floating-point coefficients that specify the scale, prebias, and postbias for the gamma curve.

`gamma`  

The power function exponent for calculating gamma correction for the gamma curve.

`linearCoeffs`  

An array of two floating-point coefficients that specify the scale and bias for the linear curve.

`boundary`  

A value that defines the boundary between the linear curve and the gamma curve.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

The piecewise gamma calculation combines a linear and an exponential (gamma) curve on two regions of the input interval, separated by a specified boundary value. When the input is greater than or equal to the boundary value, the function uses the gamma curve to generate the output; otherwise, the function uses the linear curve. This function differs from vImagePiecewiseGamma_Planar16Q12(_:_:_:_:_:_:_:) in that it’s symmetric about zero.

The following describes the operation with `x` representing the input pixel value:

```
y = fabsf(x)

if y 

## See Also

### Applying a symmetric piecewise gamma function

func vImageSymmetricPiecewiseGamma_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Float>, Float, UnsafePointer&lt;Float>, Float, vImage_Flags) -> vImage_Error

Applies a symmetric piecewise gamma function to transform a 32-bit planar image.

