

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorCubesMixedWithMask 

Protocol

# CIColorCubesMixedWithMask

The properties you use to configure a color cube mixed with mask filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorCubesMixedWithMask
```

## Topics

### Instance Properties

var colorSpace: CGColorSpace?

The working color space.

**Required**

var cube0Data: Data

The cube texture data to use as a color lookup table.

**Required**

var cube1Data: Data

The cube texture data to use as a color lookup table.

**Required**

var cubeDimension: Float

The length, in texels, of each side of the cube texture.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var maskImage: CIImage?

A masking image.

**Required**

var extrapolate: Bool

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorCubesMixedWithMask() -> any CIFilter &amp; CIColorCubesMixedWithMask

Alters an image’s pixels using a three-dimensional color tables and a mask image.

