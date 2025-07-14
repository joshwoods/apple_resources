

- Core Image
- CIFilter
- Tile Effect Filters
-  CIAffineTile 

Protocol

# CIAffineTile

The properties you use to configure an affine tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIAffineTile
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

class func affineTile() -> any CIFilter &amp; CIAffineTile

Performs a transform on the image and tiles the result.

