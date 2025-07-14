

- Accelerate
- vImage
- vImage Operations
-  Transforming with lookup tables 

API Collection

# Transforming with lookup tables

Use lookup tables to apply color transformations to images.

## Overview

Lookup table functions use the value of a source pixel as an index into a lookup table of colors that defines the corresponding destination pixel. You can use lookup table functions to perform tasks, such as color grading, converting between color spaces, or generating false-color images.

## Topics

### Transforming planar-to-planar with a lookup table

func vImageTableLookUp_Planar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an 8-bit planar image.

func vImageLookupTable_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 32-bit planar image to an 8-bit planar image.

func vImageLookupTable_Planar8toPlanar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an unsigned 16-bit planar image.

func vImageLookupTable_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 32-bit planar image.

func vImageLookupTable_8to64U(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt64>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 64-bit planar image.

func vImageLookupTable_Planar16(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_16U>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform a 16-bit planar image.

func vImageInterpolatedLookupTable_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_F>, vImagePixelCount, Float, Float, vImage_Flags) -> vImage_Error

Uses an interpolated lookup table to transform a 32-bit planar image.

### Transforming planar-to-interleaved with a lookup table

func vImageLookupTable_Planar8toPlanar24(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt32>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to an 8-bit-per-channel, three-channel interleaved image.

func vImageLookupTable_Planar8toPlanar48(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;UInt64>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 16-bit-per-channel, three-channel interleaved image.

func vImageLookupTable_Planar8toPlanar96(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_FFFF>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, three-channel interleaved image.

func vImageLookupTable_Planar8toPlanar128(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_FFFF>, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an 8-bit planar image to a 32-bit-per-channel, four-channel interleaved image.

### Transforming interleaved-to-interleaved with a lookup table

func vImageTableLookUp_ARGB8888(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;Pixel_8>!, UnsafePointer&lt;Pixel_8>!, UnsafePointer&lt;Pixel_8>!, UnsafePointer&lt;Pixel_8>!, vImage_Flags) -> vImage_Error

Uses a lookup table to transform an interleaved, four-channel 8-bit planar image to an interleaved, four-channel 8-bit planar image.

### Transforming with a multidimensional lookup table

Applying color transforms to images with a multidimensional lookup table

Precompute translation values to optimize color space conversion and other pointwise operations.

Cropping to the subject in a chroma-keyed image

Convert a chroma-key color to alpha values and trim transparent pixels using Accelerate.

Applying transformations to selected colors in an image

Desaturate a range of colors in an image with a multidimensional lookup table.

func vImageMultidimensionalTable_Create(UnsafePointer&lt;UInt16>, UInt32, UInt32, UnsafePointer&lt;UInt8>, vImageMDTableUsageHint, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> vImage_MultidimensionalTable!

Creates a multidimensional lookup table.

func vImageMultiDimensionalInterpolatedLookupTable_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_MultidimensionalTable, vImage_InterpolationMethod, vImage_Flags) -> vImage_Error

Uses a multidimensional lookup table to transform a 32-bit planar image.

func vImageMultiDimensionalInterpolatedLookupTable_Planar16Q12(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, UnsafeMutableRawPointer!, vImage_MultidimensionalTable, vImage_InterpolationMethod, vImage_Flags) -> vImage_Error

Uses a multidimensional lookup table to transform a 16Q12 planar image.

func vImageMultidimensionalTable_Retain(vImage_MultidimensionalTable!) -> vImage_Error

Retains a multidimensional table.

func vImageMultidimensionalTable_Release(vImage_MultidimensionalTable!) -> vImage_Error

Releases a multidimensional table.

typealias vImage_MultidimensionalTable

An opaque pointer that represents a multidimensional lookup table.

struct vImageMDTableUsageHint

Constants that indicate the use for a multidimensional lookup table.

struct vImage_InterpolationMethod

Constants that represent different interpolation methods.

## See Also

### Applying color transforms to images

Transforming with polynomials

Use polynomials to apply color transformations to images.

Transforming with matrix multiplication

Use matrix multiplication to apply color transformations to images.

Transforming with a gamma function

Use gamma functions to apply color transformations to images.

Applying a flood fill to an image

Fill connected components of an image with a new color.

