

- Core Image
- CIFilter
- Stylizing Filters
-  CIHexagonalPixellate 

Protocol

# CIHexagonalPixellate

The properties you use to configure a hexagonal pixellate filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHexagonalPixellate
```

## Topics

### Instance Properties

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var scale: Float

The size of the hexagons.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func hexagonalPixellate() -> any CIFilter &amp; CIHexagonalPixellate

Creates an image made of a series of colorful hexagons.

