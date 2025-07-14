

- Accelerate
-  vImageCreateGammaFunction(\_:\_:\_:) 

Function

# vImageCreateGammaFunction(\_:\_:\_:)

Returns a gamma function object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCreateGammaFunction(
    _ gamma: Float,
    _ gamma_type: Int32,
    _ flags: vImage_Flags
) -> GammaFunction!
```

## Parameters 

`gamma`  

The gamma value when `gamma_type` is kvImageGamma_UseGammaValue or kvImageGamma_UseGammaValue_half_precision.

`gamma_type`  

A constant that specifies the gamma type. See Gamma function types.

`flags`  

Reserved for future use. Pass kvImageNoFlags.

## Return Value

A gamma function object that encapsulates a gamma value, a gamma function type, and option flags.

## Discussion

Use this function to create a gamma function object that you pass to vImageGamma_Planar8toPlanarF(_:_:_:_:), vImageGamma_PlanarFtoPlanar8(_:_:_:_:), or vImageGamma_PlanarF(_:_:_:_:).

The vImage library provides a user-defined half-precision gamma type and constant half-precision gamma types, such as kvImageGamma_sRGB_forward_half_precision. Use a half-precision gamma type when creating a gamma function for image data that’s intended for conversion to 8-bit. The half-precision gamma types work with floating-point values in the range `0...1` and provide a precision of ±1 / 4,096.

The gamma correction functions that use a GammaFunction object are symmetric around zero. That is, they treat negative values as if they’re positive, and restore the sign after applying the exponent.

## See Also

### Applying a gamma function

Gamma function types

Types of full- or half-precision gamma functions.

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

