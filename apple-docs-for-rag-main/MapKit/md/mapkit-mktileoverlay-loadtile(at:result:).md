

- MapKit
- MKTileOverlay
-  loadTile(at:result:) 

Instance Method

# loadTile(at:result:)

Loads the specified tile asynchronously.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func loadTile(
    at path: MKTileOverlayPath,
    result: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func loadTile(at path: MKTileOverlayPath) async throws -> Data
```

## Parameters 

`path`  

The path structure that identifies the specific tile you want. This structure incorporates the tile’s x-y coordinate at a given zoom level and scale factor.

`result`  

The completion block to call when the tile data is available. The method can execute this block on any queue and takes the following parameters:

- The `tileData` parameter contains the raw data that loads from the corresponding image file. You can use this data to initialize an image object. If an error occurs, this parameter is `nil`.

- The `error` parameter contains an error object if there is a problem loading the tile image. If no errors occur, this parameter is `nil`.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func loadTile(at path: MKTileOverlayPath) async throws -> Data
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The default implementation of this method uses the url(forTilePath:) method to retrieve the URL for the specified tile and then loads that tile into memory asynchronously using a URLSession object. The specified tile may be located either on the local file system or on a remote server. Subclasses may override this method and implement their own custom tile-loading behavior.

When a tile overlay renderer (that is, an instance of MKTileOverlayRenderer) needs to display tiles, it uses this method to request the data for each tile.

## See Also

### Customizing the loading of tiles

var urlTemplate: String?

The template for generating tile image URLs.

func url(forTilePath: MKTileOverlayPath) -> URL

Returns the URL to use to access the specified tile.

struct MKTileOverlayPath

Values that specify the path indexes for a single overlay tile.

