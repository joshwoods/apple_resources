

- MapKit
- MKTileOverlay
-  url(forTilePath:) 

Instance Method

# url(forTilePath:)

Returns the URL to use to access the specified tile.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func url(forTilePath path: MKTileOverlayPath) -> URL
```

## Parameters 

`path`  

The path structure that identifies the specific tile you want. This structure incorporates the tile’s x-y coordinate at a given zoom level and scale factor.

## Return Value

The URL to use to retrieve the tile.

## Discussion

The default implementation of this method uses the template string you provide at initialization time to build a URL to the specified tile image. Subclasses can override this method and use a different scheme to provide URLs for tiles. You can locate the tiles either on a local file system or on a remote server.

## See Also

### Related Documentation

init(urlTemplate: String?)

Creates and returns a tile overlay object using the specified tile-access template.

### Customizing the loading of tiles

var urlTemplate: String?

The template for generating tile image URLs.

func loadTile(at: MKTileOverlayPath, result: (Data?, (any Error)?) -> Void)

Loads the specified tile asynchronously.

struct MKTileOverlayPath

Values that specify the path indexes for a single overlay tile.

