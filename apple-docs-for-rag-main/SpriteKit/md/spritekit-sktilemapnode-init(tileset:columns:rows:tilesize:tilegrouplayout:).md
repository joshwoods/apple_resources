

- SpriteKit
- SKTileMapNode
-  init(tileSet:columns:rows:tileSize:tileGroupLayout:) 

Initializer

# init(tileSet:columns:rows:tileSize:tileGroupLayout:)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows. For a grid set type, the overall size, in points, of the node will be `numberOfColumns * tileSize.width` wide and `numberOfRows * tileSize.height` high.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
init(
    tileSet: SKTileSet,
    columns: Int,
    rows: Int,
    tileSize: CGSize,
    tileGroupLayout: [SKTileGroup]
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(
    tileSet: SKTileSet,
    columns: Int,
    rows: Int,
    tileSize: CGSize,
    tileGroupLayout: [SKTileGroup]
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

`tileGroupLayout`  

An array of tile groups to fill the tile map with.

## Return Value

A new tile map node.

## Discussion

This initializer fills each tile with a texture defined by the final argument which is a row-major array of SKTileGroup objects. For example, for a 2 by 2 map node, a `tileGroupLayout` of `[A, B, C, D]` would place tile group `A` in the bottom left of the node and group `D` in the top right. The length of the tile group layout array should be the same as columns multiplied by rows.

## See Also

### Creating a Tile Map

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

init(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, fillWith: SKTileGroup)

Creates and initializes a tile map node using the provided tile set with a specified number of columns and rows.

class func tileMapNodes(tileSet: SKTileSet, columns: Int, rows: Int, tileSize: CGSize, from: GKNoiseMap, tileTypeNoiseMapThresholds: [NSNumber]) -> [SKTileMapNode]

Creates a tile map node by allowing a GKNoiseMap to choose its tiles.

