

- MapKit
- MKTileOverlay
-  canReplaceMapContent 

Instance Property

# canReplaceMapContent

A Boolean value that indicates whether the tile content is fully opaque.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var canReplaceMapContent: Bool { get set }
```

## Discussion

If the tile content you provide can cover the entire drawing area with opaque content, set this property to true. Doing so serves as a hint to the map view that it doesn’t need to draw any additional content underneath your tiles. Set this property to false if your tiles contain any transparency.

The default value for this property is false.

## See Also

### Accessing the tile attributes

var tileSize: CGSize

The size (in pixels) of your tile images.

var isGeometryFlipped: Bool

A Boolean value that indicates the orientation of tile indexes along the y-axis.

var minimumZ: Int

The minimum zoom level that the tiles of this overlay object support.

var maximumZ: Int

The maximum zoom level that the tiles of this overlay object support.

