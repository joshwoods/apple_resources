

- Core Image
- CIFilter
- Tile Effect Filters
-  CIParallelogramTile 

Protocol

# CIParallelogramTile

The properties you use to configure a parallelogram tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIParallelogramTile
```

## Topics

### Instance Properties

var acuteAngle: Float

The primary angle for the repeating parallelogram tile.

**Required**

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

class func parallelogramTile() -> any CIFilter &amp; CIParallelogramTile

Warps the image to create a parallelogram and tiles the result.

