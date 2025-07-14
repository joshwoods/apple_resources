

- Accelerate
-  kvImageConvert_DitherFloydSteinberg 

Global Variable

# kvImageConvert_DitherFloydSteinberg

A constant that indicates the conversion will add Floyd-Steinberg dithering to the image.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kvImageConvert_DitherFloydSteinberg: UInt32 { get }
```

## Discussion

The following shows an 8-bit RGB image converted to a 1-bit planar image with vImageConvert_Planar8toPlanar1(_:_:_:_:_:) using kvImageConvert_DitherFloydSteinberg:

To learn about converting an RGB image to grayscale, see Converting color images to grayscale.

## See Also

### Constants

var kvImageConvert_DitherNone: UInt32

A constant that indicates the conversion will not apply dithering.

var kvImageConvert_DitherOrdered: UInt32

A constant that indicates the conversion will add randomized, pre-computed blue noise to the image.

var kvImageConvert_DitherOrderedReproducible: UInt32

A constant that indicates the conversion will add reproducible, pre-computed blue noise to the image.

var kvImageConvert_DitherAtkinson: UInt32

A constant that indicates the conversion will add Atkinson dithering to the image.

var kvImageConvert_OrderedGaussianBlue: UInt32

A constant that indicates the conversion will distribute the noise according to a Gaussian distribution.

var kvImageConvert_OrderedUniformBlue: UInt32

A constant that indicates the conversion will distribute the noise uniformly.

var kvImageConvert_OrderedNoiseShapeMask: UInt32

