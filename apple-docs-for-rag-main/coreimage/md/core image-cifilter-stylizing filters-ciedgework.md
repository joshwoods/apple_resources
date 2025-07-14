

- Core Image
- CIFilter
- Stylizing Filters
-  CIEdgeWork 

Protocol

# CIEdgeWork

The properties you use to configure an edge-work filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIEdgeWork
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The thickness of the edges.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func edgeWork() -> any CIFilter &amp; CIEdgeWork

Produces a black-and-white image that looks similar to a woodblock print.

