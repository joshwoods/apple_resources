

- AppKit
- NSApplication
-  applicationIconImage 

Instance Property

# applicationIconImage

The image used for the app’s icon.

macOS

``` source
@MainActor
var applicationIconImage: NSImage! { get set }
```

## Discussion

Assign an image to this property when you want to temporarily change the app icon in the dock app tile. The image you provide is scaled as needed so that it fits in the tile. To restore your app’s original icon, set this property to `nil`.

## See Also

### Accessing the Dock Tile

var dockTile: NSDockTile

The app’s Dock tile.

