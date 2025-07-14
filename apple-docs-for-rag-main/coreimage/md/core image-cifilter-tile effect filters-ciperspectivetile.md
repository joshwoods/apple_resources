

- Core Image
- CIFilter
- Tile Effect Filters
-  CIPerspectiveTile 

Protocol

# CIPerspectiveTile

The properties you use to configure a perspective tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPerspectiveTile
```

## Topics

### Instance Properties

var bottomLeft: CGPoint

The bottom-left coordinate of a tile.

**Required**

var bottomRight: CGPoint

The bottom-right coordinate of a tile.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var topLeft: CGPoint

The top-left coordinate of a tile.

**Required**

var topRight: CGPoint

The top-right coordinate of a tile.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func perspectiveTile() -> any CIFilter &amp; CIPerspectiveTile

Tiles an image by adjusting the perspective of the image.

