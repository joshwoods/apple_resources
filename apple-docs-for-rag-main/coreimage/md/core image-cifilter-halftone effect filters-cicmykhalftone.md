

- Core Image
- CIFilter
- Halftone Effect Filters
-  CICMYKHalftone 

Protocol

# CICMYKHalftone

The properties you use to configure a CMYK halftone filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICMYKHalftone
```

## Topics

### Instance Properties

var angle: Float

The angle of the pattern.

**Required**

var center: CGPoint

The x and y position to use as the center of the halftone pattern.

**Required**

var grayComponentReplacement: Float

The gray component replacement value.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var sharpness: Float

The sharpness of the pattern.

**Required**

var underColorRemoval: Float

The under color removal value.

**Required**

var width: Float

The distance between dots in the pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func cmykHalftone() -> any CIFilter &amp; CICMYKHalftone

Adds a series of colorful dots to an image.

