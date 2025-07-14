

- SpriteKit
- SKTileMapNode
-  tileMapNodes(tileSet:columns:rows:tileSize:from:tileTypeNoiseMapThresholds:) 

Type Method

# tileMapNodes(tileSet:columns:rows:tileSize:from:tileTypeNoiseMapThresholds:)

Creates a tile map node by allowing a GKNoiseMap to choose its tiles.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
@MainActor
class func tileMapNodes(
    tileSet: SKTileSet,
    columns: Int,
    rows: Int,
    tileSize: CGSize,
    from noiseMap: GKNoiseMap,
    tileTypeNoiseMapThresholds thresholds: [NSNumber]
) -> [SKTileMapNode]
```

## See Also

### Creating a Tile Map

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, fillWith: SKTileGroup)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, tileGroupLayout: [SKTileGroup])

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows. For a grid set type, the overall size, in points, of the node will be `numberOfColumns * tileSize.width` wide and `numberOfRows * tileSize.height` high.

