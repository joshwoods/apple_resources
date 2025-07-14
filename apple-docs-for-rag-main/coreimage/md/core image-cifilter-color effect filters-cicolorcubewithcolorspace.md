

- Core Image
- CIFilter
- Color Effect Filters
-  CIColorCubeWithColorSpace 

Protocol

# CIColorCubeWithColorSpace

The properties you use to configure a color cube with color space filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorCubeWithColorSpace
```

## Topics

### Instance Properties

var colorSpace: CGColorSpace?

The working color space.

**Required**

var cubeData: Data

The cube texture data to use as a color lookup table.

**Required**

var cubeDimension: Float

The length, in texels, of each side of the cube texture.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var extrapolate: Bool

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorCubeWithColorSpace() -> any CIFilter &amp; CIColorCubeWithColorSpace

Adjusts an image’s pixels using a three-dimensional color table in specified color space.

