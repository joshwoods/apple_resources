

- Core Image
- CIFilter
- Tile Effect Filters
-  CIFourfoldTranslatedTile 

Protocol

# CIFourfoldTranslatedTile

The properties you use to configure a fourfold translated tile filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIFourfoldTranslatedTile
```

## Topics

### Instance Properties

var acuteAngle: Float

The primary angle for the repeating translated tile.

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

class func fourfoldTranslatedTile() -> any CIFilter &amp; CIFourfoldTranslatedTile

Creates a tiled image by applying four translation operations.

