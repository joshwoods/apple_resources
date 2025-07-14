

- Core Image
- CIFilter
- Tile Effect Filters
-  CIOpTile 

Protocol

# CIOpTile

The properties you use to configure an optical tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIOpTile
```

## Topics

### Instance Properties

var angle: Float

The angle of a tile.

**Required**

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var scale: Float

A value that determines the number of tiles in the effect.

**Required**

var width: Float

The width of a tile.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func opTile() -> any CIFilter &amp; CIOpTile

Produces an effect that mimics a style of visual art that uses optical illusions.

