

- SpriteKit
- SKTileMapNode
-  tileSet 

Instance Property

# tileSet

The tile set being used by this tile map. The tile map object can only display tiles that exist in this set.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
var tileSet: SKTileSet { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var tileSet: SKTileSet { get set }
```

## See Also

### Reading or Manually Configuring the Tile Map’s Size

var tileSize: CGSize

The size of each tile in points.

var numberOfColumns: Int

The number of columns in the tile map

var numberOfRows: Int

The number of rows in the tile map.

