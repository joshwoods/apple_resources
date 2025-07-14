

- Accelerate
-  ResamplingFilter 

Type Alias

# ResamplingFilter

A pointer to a resampling filter callback function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias ResamplingFilter = UnsafeMutableRawPointer
```

## Discussion

You pass a resampling filter callback to a shear function. The resampling filter pointer can point to a structure that contains a function, rows of precalculated values, flag settings, and so on. The shear function requires that the structure contains a scale factor.

## See Also

### Data Types

struct vImage_Buffer

An image buffer that stores an image’s pixel data, dimensions, and row stride.

typealias vImagePixelCount

A type for the number of pixels.

struct vImage_AffineTransform

A structure for values that represent an affine transformation.

struct vImage_AffineTransform_Double

A structure for values that represent a double-precision affine transformation.

typealias vImage_CGAffineTransform

A structure for values that represent a Core Graphics–compatible affine transformation.

typealias vImage_Error

A type for image errors.

typealias vImage_Flags

A type for processing options.

typealias GammaFunction

A type for a gamma function.

