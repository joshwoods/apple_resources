

- AppKit
- NSDockTile
-  size 

Instance Property

# size

The size of the tile.

macOS 10.5+

``` source
var size: NSSize { get }
```

## Discussion

This corresponds to the size of the backing store in the dock, which may be bigger than the actual tile displayed on the screen.

## See Also

### Getting the Tile Information

var owner: AnyObject?

The object represented by the dock tile.

