

- Core Image
- CIFilter
- Stylizing Filters
-  CIPointillize 

Protocol

# CIPointillize

The properties you use to configure a pointillize filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPointillize
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius of the circles in the resulting pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func pointillize() -> any CIFilter &amp; CIPointillize

Applies a pointillize effect to an image.

