

- Accelerate
- vImage
- vImage Operations
-  Transforming with polynomials 

API Collection

# Transforming with polynomials

Use polynomials to apply color transformations to images.

## Overview

Polynomial functions apply one or more polynomials to the input image to generate the output image. You can use polynomial functions to apply tone curve adjustments to images.

## Topics

### Applying a polynomial

Applying tone curve adjustments to images

Use the vImage library’s polynomial transform to apply tone curve adjustments to images.

func vImagePiecewisePolynomial_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise polynomials to transform an 8-bit planar image to a 32-bit planar image.

func vImagePiecewisePolynomial_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise polynomials to transform a 32-bit planar image to an 8-bit planar image.

func vImagePiecewisePolynomial_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise polynomials to transform a 32-bit planar image.

### Applying a symmetric polynomial

func vImageSymmetricPiecewisePolynomial_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of symmetric piecewise polynomials to transform a 32-bit planar image.

### Applying a rational expression

func vImagePiecewiseRational_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafeMutablePointer&lt;UnsafePointer&lt;Float>?>, UnsafePointer&lt;Float>, UInt32, UInt32, UInt32, vImage_Flags) -> vImage_Error

Applies a set of piecewise rational expressions to transform a 32-bit planar image.

## See Also

### Applying color transforms to images

Transforming with lookup tables

Use lookup tables to apply color transformations to images.

Transforming with matrix multiplication

Use matrix multiplication to apply color transformations to images.

Transforming with a gamma function

Use gamma functions to apply color transformations to images.

Applying a flood fill to an image

Fill connected components of an image with a new color.

