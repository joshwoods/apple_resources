

- MapKit
- MKTileOverlay
-  urlTemplate 

Instance Property

# urlTemplate

The template for generating tile image URLs.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
var urlTemplate: String? { get }
```

## Discussion

You specify this string at initialization time.

## See Also

### Related Documentation

init(urlTemplate: String?)

Creates and returns a tile overlay object using the specified tile-access template.

### Customizing the loading of tiles

func url(forTilePath: MKTileOverlayPath) -> URL

Returns the URL to use to access the specified tile.

func loadTile(at: MKTileOverlayPath, result: (Data?, (any Error)?) -> Void)

Loads the specified tile asynchronously.

struct MKTileOverlayPath

Values that specify the path indexes for a single overlay tile.

