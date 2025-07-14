

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIColorPolynomial 

Protocol

# CIColorPolynomial

The properties you use to configure a color polynomial filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorPolynomial
```

## Topics

### Instance Properties

var alphaCoefficients: CIVector

Polynomial coefficients for the alpha channel.

**Required**

var blueCoefficients: CIVector

Polynomial coefficients for the blue channel.

**Required**

var greenCoefficients: CIVector

Polynomial coefficients for the green channel.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var redCoefficients: CIVector

Polynomial coefficients for the red channel.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorPolynomial() -> any CIFilter &amp; CIColorPolynomial

Alters an image’s colors.

