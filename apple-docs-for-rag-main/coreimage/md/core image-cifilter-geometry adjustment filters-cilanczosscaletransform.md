

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CILanczosScaleTransform 

Protocol

# CILanczosScaleTransform

The properties you use to configure a Lanczos scale transform filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILanczosScaleTransform
```

## Topics

### Instance Properties

var aspectRatio: Float

The additional horizontal scaling factor to use on the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var scale: Float

The scaling factor to use on the image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func lanczosScaleTransform() -> any CIFilter &amp; CILanczosScaleTransform

Creates a high-quality, scaled version of a source image.

