

- SpriteKit
- SKTileMapNode
-  centerOfTile(atColumn:row:) 

Instance Method

# centerOfTile(atColumn:row:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func centerOfTile(
    atColumn column: Int,
    row: Int
) -> CGPoint
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func centerOfTile(
    atColumn column: Int,
    row: Int
) -> CGPoint
```

## Parameters 

`column`  

The column index of the tile.

`row`  

The row index of the tile.

## Return Value

The coordinates in points of the center of the tile for a given column and row.

## See Also

### Querying the Tile Map’s Properties

func tileColumnIndex(fromPosition: CGPoint) -> Int

func tileDefinition(atColumn: Int, row: Int) -> SKTileDefinition?

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

func tileRowIndex(fromPosition: CGPoint) -> Int

Returns the tile map node object’s tile row index for the specified position in points.

var mapSize: CGSize

The overall size of the tile map.

