

- Core Image
- CIFilter
- Tile Effect Filters
-  CIAffineClamp 

Protocol

# CIAffineClamp

The properties you use to configure an affine clamp filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIAffineClamp
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var transform: CGAffineTransform

The transform to apply to the image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func affineClamp() -> any CIFilter &amp; CIAffineClamp

Performs a transform on the image and extends the image edges to infinity.

