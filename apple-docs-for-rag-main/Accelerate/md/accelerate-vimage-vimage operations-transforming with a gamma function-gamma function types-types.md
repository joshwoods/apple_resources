

- Accelerate
- vImage
- vImage Operations
- Transforming with a gamma function
-  Gamma function types 

API Collection

# Gamma function types

Types of full- or half-precision gamma functions.

## Topics

### User-defined gamma values

var kvImageGamma_UseGammaValue: Int

A user-defined gamma value with full-precision calculation.

var kvImageGamma_UseGammaValue_half_precision: Int

A user-defined gamma value with half-precision calculation.

### Constant gamma values

var kvImageGamma_BT709_forward_half_precision: Int

The ITU-R BT.709 standard.

var kvImageGamma_BT709_reverse_half_precision: Int

The ITU-R BT.709 standard reverse.

var kvImageGamma_sRGB_forward_half_precision: Int

A half-precision calculation using the sRGB standard gamma value of 2.2.

var kvImageGamma_sRGB_reverse_half_precision: Int

A half-precision calculation using the sRGB standard gamma value of 1/2.2.

var kvImageGamma_5_over_9_half_precision: Int

A half-precision calculation using a gamma value of 5/9 or 1/1.8.

var kvImageGamma_5_over_11_half_precision: Int

A half-precision calculation using a gamma value of 5/11 or 1/2.2.

var kvImageGamma_9_over_5_half_precision: Int

A half-precision calculation using a gamma value of 9/5 or 1.8.

var kvImageGamma_9_over_11_half_precision: Int

A half-precision calculation using a gamma value of 9/11 or (9/5)/(11/5).

var kvImageGamma_11_over_5_half_precision: Int

A half-precision calculation using a gamma value of 11/5 or 2.2.

var kvImageGamma_11_over_9_half_precision: Int

A half-precision calculation using a gamma value of 11/9 or (11/5)/(9/5).

## See Also

### Applying a gamma function

func vImageCreateGammaFunction(Float, Int32, vImage_Flags) -> GammaFunction!

Returns a gamma function object.

func vImageGamma_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to an 8-bit planar image to produce a 32-bit planar image.

func vImageGamma_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a 32-bit planar image to produce an 8-bit planar image.

func vImageGamma_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a PlanarF image.

func vImageDestroyGammaFunction(GammaFunction!)

Destroys a gamma function object.

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

