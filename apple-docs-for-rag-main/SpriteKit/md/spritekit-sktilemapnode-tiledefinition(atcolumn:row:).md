

- SpriteKit
- SKTileMapNode
-  tileDefinition(atColumn:row:) 

Instance Method

# tileDefinition(atColumn:row:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func tileDefinition(
    atColumn column: Int,
    row: Int
) -> SKTileDefinition?
```

**watchOS**

``` source
func tileDefinition(
    atColumn column: Int,
    row: Int
) -> SKTileDefinition?
```

## Parameters 

`column`  

The column index of the tile.

`row`  

The row index of the tile.

## Return Value

The tile definition for the tile at the specified column and row.

## See Also

### Querying the Tile Map’s Properties

func centerOfTile(atColumn: Int, row: Int) -> CGPoint

func tileColumnIndex(fromPosition: CGPoint) -> Int

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

func tileRowIndex(fromPosition: CGPoint) -> Int

Returns the tile map node object’s tile row index for the specified position in points.

var mapSize: CGSize

The overall size of the tile map.

