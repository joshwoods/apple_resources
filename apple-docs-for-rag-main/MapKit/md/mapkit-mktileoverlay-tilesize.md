

- MapKit
- MKTileOverlay
-  tileSize 

Instance Property

# tileSize

The size (in pixels) of your tile images.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var tileSize: CGSize { get set }
```

## Discussion

On Retina displays, the system renders images pixel for pixel and doesn’t scale them. This means that if the tile size is 256 x 256 pixels and the scale factor is `2.0`, the system renders the image as if it is 128 x 128 points in size. This behavior causes the tile to appear smaller, but preserves the original image data.

The default tile size is 256 x 256 pixels.

## See Also

### Accessing the tile attributes

var isGeometryFlipped: Bool

A Boolean value that indicates the orientation of tile indexes along the y-axis.

var minimumZ: Int

The minimum zoom level that the tiles of this overlay object support.

var maximumZ: Int

The maximum zoom level that the tiles of this overlay object support.

var canReplaceMapContent: Bool

A Boolean value that indicates whether the tile content is fully opaque.

