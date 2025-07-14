

- Accelerate
-  vImageDestroyGammaFunction(\_:) 

Function

# vImageDestroyGammaFunction(\_:)

Destroys a gamma function object.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOS 5.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageDestroyGammaFunction(_ f: GammaFunction!)
```

## Parameters 

`f`  

The gamma function object.

## See Also

### Applying a gamma function

func vImageCreateGammaFunction(Float, Int32, vImage_Flags) -> GammaFunction!

Returns a gamma function object.

Gamma function types

Types of full- or half-precision gamma functions.

func vImageGamma_Planar8toPlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to an 8-bit planar image to produce a 32-bit planar image.

func vImageGamma_PlanarFtoPlanar8(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a 32-bit planar image to produce an 8-bit planar image.

func vImageGamma_PlanarF(UnsafePointer&lt;vImage_Buffer>, UnsafePointer&lt;vImage_Buffer>, GammaFunction!, vImage_Flags) -> vImage_Error

Applies a gamma function to a PlanarF image.

Adjusting saturation and applying tone mapping

Convert an RGB image to discrete luminance and chrominance channels, and apply color and contrast treatments.

