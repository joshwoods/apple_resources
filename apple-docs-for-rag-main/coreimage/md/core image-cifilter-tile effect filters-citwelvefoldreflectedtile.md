

- Core Image
- CIFilter
- Tile Effect Filters
-  CITwelvefoldReflectedTile 

Protocol

# CITwelvefoldReflectedTile

The properties you use to configure a twelvefold reflected tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CITwelvefoldReflectedTile
```

## Topics

### Instance Properties

var angle: Float

The angle, in radians, of the tiled pattern.

**Required**

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var width: Float

The width of a tile.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func twelvefoldReflectedTile() -> any CIFilter &amp; CITwelvefoldReflectedTile

Creates a tiled image by rotating in increments of 30 degrees.

