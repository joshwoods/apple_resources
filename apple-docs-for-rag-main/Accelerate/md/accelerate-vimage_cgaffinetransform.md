

- Accelerate
-  vImage_CGAffineTransform 

Type Alias

# vImage_CGAffineTransform

A structure for values that represent a Core Graphics–compatible affine transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias vImage_CGAffineTransform = vImage_AffineTransform_Double
```

## Mentioned in 

Applying geometric transforms to images

## Discussion

This structure represents the 3x2 matrix :

This structure changes size to be the same size as the Core Graphics CGAffineTransform data structure. CGAffineTransform describes functions for creating and manipulating matrixes of this form.

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

typealias vImage_Error

A type for image errors.

typealias vImage_Flags

A type for processing options.

typealias GammaFunction

A type for a gamma function.

typealias ResamplingFilter

A pointer to a resampling filter callback function.

