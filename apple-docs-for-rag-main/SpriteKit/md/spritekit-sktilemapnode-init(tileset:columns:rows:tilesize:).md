

- SpriteKit
- SKTileMapNode
-  init(tileSet:columns:rows:tileSize:) 

Initializer

# init(tileSet:columns:rows:tileSize:)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
init(
    tileSet: SKTileSet,
    columns: Int,
    rows: Int,
    tileSize: CGSize
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(
    tileSet: SKTileSet,
    columns: Int,
    rows: Int,
    tileSize: CGSize
)
```

## Parameters 

`tileSet`  

The tile set that is used to render the tiles

`columns`  

The number of columns in the map

`rows`  

The number of rows in the map

`tileSize`  

The size of each tile in points

## Return Value

A new tile map node.

## Discussion

Creates an empty tile map.

For a grid set type, the overall size in points of the node will be `numberOfColumns` \* `tileSize.width` wide and `numberOfRows` \* `tileSize.height` high.

## See Also

### Creating a Tile Map

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, fillWith: SKTileGroup)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, tileGroupLayout: [SKTileGroup])

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows. For a grid set type, the overall size, in points, of the node will be `numberOfColumns * tileSize.width` wide and `numberOfRows * tileSize.height` high.

class func tileMapNodes(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, from: GKNoiseMap, tileTypeNoiseMapThresholds: [NSNumber]) -> [SKTileMapNode]

Creates a tile map node by allowing a GKNoiseMap to choose its tiles.

