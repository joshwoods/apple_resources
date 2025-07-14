

- Accelerate
-  vImagePiecewisePolynomial_PlanarF(\_:\_:\_:\_:\_:\_:\_:) 

Function

# vImagePiecewisePolynomial_PlanarF(\_:\_:\_:\_:\_:\_:\_:)

Applies a set of piecewise polynomials to transform a 32-bit planar image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImagePiecewisePolynomial_PlanarF(
    _ src: UnsafePointer,
    _ dest: UnsafePointer,
    _ coefficients: UnsafeMutablePointer?>,
    _ boundaries: UnsafePointer,
    _ order: UInt32,
    _ log2segments: UInt32,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`src`  

The source vImage buffer.

`dest`  

A pointer to the destination vImage buffer structure. You’re responsible for filling out the `height`, `width`, and `rowBytes` fields of this structure, and for allocating a data buffer of the appropriate size. On return, the data buffer this structure points to contains the destination image data. When you no longer need the data buffer, deallocate the memory to prevent memory leaks.

`coefficients`  

A pointer to an array of polynomial coefficient arrays. Each polynomial coefficient array contains the coefficients for one polynomial. A polynomial of order `R` has `R+1` coefficients, and all of the polynomials in this array must have the same order.

Order the coefficients from the zeroth-order term to the highest order term. For example, the function evaluates the coefficients `[0.5, 0.6, 0.7]` as `0.5 * x⁰ + 0.6 * x¹ + 0.7 * x²`.

`boundaries`  

A pointer to an array of boundary values, in increasing order, that separates adjacent ranges of pixel values. The first boundary value is the lowest in the range and the function clips input values lower than this to this value. The last boundary value is the highest in the range and the function clips input values higher than this to this value. The boundary values between the first and last separate the subranges from each other.

`order`  

The order of the polynomials.

`log2segments`  

The number of polynomials to represent as a base-2 logarithm. If you pass a noninteger power-of-two number of polynomials, round up to the next integer power of two, and repeat the last polynomial the appropriate number of times.

`flags`  

The options to use when performing the operation. If your code implements its own tiling or its own multithreading, pass kvImageDoNotTile; otherwise, pass kvImageNoFlags.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

You can approximate many different correction functions by carefully choosing the polynomials and the ranges of input values they operate on. For example, the sample code project Applying tone curve adjustments to images demonstrates how to apply tone curve adjustments to images using polynomial transforms.

The following code defines two sets of polynomial coefficients, `coefficients0` as `[0.0, 0.5, 0.0]` and `coefficients1` as `[0.0, 0.0, 1.0].` The boundaries array, `[0, 0.5, 1]`, specifies that the vImagePiecewisePolynomial_PlanarF(_:_:_:_:_:_:_:) function applies `coefficients0` to source pixels less than `0.5`, and applies `coefficients1` to other pixels.

Note that the boundaries array contains three elements that define two ranges: `0..

```
let source = vImage.PixelBuffer(
    pixelValues: [0, 0.2, 0.4, 0.6, 0.8, 1],
    size: vImage.Size(width: 6, height: 1))

let destination = vImage.PixelBuffer(
    size: source.size)

let coefficients0: [Float] = [0.0, 0.5, 0.0] // 0.0 * x⁰ + 0.5 * x¹ + 0.0 * x²
let coefficients1: [Float] = [0.0, 0.0, 1.0] // 0.0 * x⁰ + 0.0 * x¹ + 1.0 * x²

let boundaries: [Float] = [0, 0.5, 1]

let order = UInt32(2)

let log2segments = UInt32(1)

coefficients0.withUnsafeBufferPointer { coefficients0Ptr in
    coefficients1.withUnsafeBufferPointer { coefficients1Ptr in
        source.withUnsafePointerToVImageBuffer { src in
            destination.withUnsafePointerToVImageBuffer { dest in

                var coeffs = [ coefficients0Ptr.baseAddress,
                               coefficients1Ptr.baseAddress ]

                vImagePiecewisePolynomial_PlanarF(
                    src,
                    dest,
                    &coeffs,
                    boundaries,
                    order,
                    log2segments,
                    vImage_Flags(kvImageNoFlags))
            }
        }
    }
}
```

On return, the destination buffer contains the values `[0.0, 0.1, 0.2, 0.36, 0.64, 1.0]`. This is equivalent to the following scalar code:

```
let result = source.array.map { x in
    let coefficients = x 

For best performance, choose a single higher-order polynomial over many lower-order polynomials. However, this function uses single-precision arithmetic, and large high-order coefficients may cause rounding errors.

## See Also

### Applying a polynomial

Applying tone curve adjustments to images

Use the vImage library’s polynomial transform to apply tone curve adjustments to images.

func vImagePiecewisePolynomial_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise polynomials to transform an 8-bit planar image to a 32-bit planar image.

func vImagePiecewisePolynomial_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise polynomials to transform a 32-bit planar image to an 8-bit planar image.

