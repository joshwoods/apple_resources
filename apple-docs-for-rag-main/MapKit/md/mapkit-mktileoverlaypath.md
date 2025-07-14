

- MapKit
-  MKTileOverlayPath 

Structure

# MKTileOverlayPath

Values that specify the path indexes for a single overlay tile.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MKTileOverlayPath
```

## Topics

### Creating a tile overlay path

init()

Creates a new tile overlay path.

init(x: Int, y: Int, z: Int, contentScaleFactor: CGFloat)

Creates a new overlay path with the specified indexes and content scale factor.

### Instance properties

var x: Int

The index of the tile along the x-axis of the map.

var y: Int

The index of the tile along the y-axis of the map.

var z: Int

The index of the tile along the z-axis of the map.

var contentScaleFactor: CGFloat

The tile’s intended screen scale factor.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Customizing the loading of tiles

var urlTemplate: String?

The template for generating tile image URLs.

func url(forTilePath: MKTileOverlayPath) -> URL

Returns the URL to use to access the specified tile.

func loadTile(at: MKTileOverlayPath, result: (Data?, (any Error)?) -> Void)

Loads the specified tile asynchronously.

