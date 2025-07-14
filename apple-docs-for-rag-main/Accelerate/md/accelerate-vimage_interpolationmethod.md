

- Accelerate
-  vImage_InterpolationMethod 

Structure

# vImage_InterpolationMethod

Constants that represent different interpolation methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct vImage_InterpolationMethod
```

## Topics

### Interpolation method constants

var kvImageNoInterpolation: vImage_InterpolationMethod

Nearest neighbor interpolation.

var kvImageHalfInterpolation: vImage_InterpolationMethod

Partial linear interpolation.

var kvImageFullInterpolation: vImage_InterpolationMethod

Full linear interpolation.

### Raw values

init(UInt32)

Creates an interpolation method constant with an unsigned-integer value.

init(rawValue: UInt32)

Creates an interpolation method constant with an unsigned-integer value.

var rawValue: UInt32

The raw value that represents the interpolation method constant.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

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

