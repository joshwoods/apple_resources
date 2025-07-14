

- Core Image
- CIFilter
- Stylizing Filters
-  CIEdges 

Protocol

# CIEdges

The properties you use to configure an edges filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIEdges
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the edges.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func edges() -> any CIFilter &amp; CIEdges

Hilghlights edges of objects found within an image.

