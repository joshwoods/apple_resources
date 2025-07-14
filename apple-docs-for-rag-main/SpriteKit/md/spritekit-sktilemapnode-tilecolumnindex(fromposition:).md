

- SpriteKit
- SKTileMapNode
-  tileColumnIndex(fromPosition:) 

Instance Method

# tileColumnIndex(fromPosition:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func tileColumnIndex(fromPosition position: CGPoint) -> Int
```

**watchOS**

``` source
func tileColumnIndex(fromPosition position: CGPoint) -> Int
```

## Parameters 

`position`  

The position in the tile map to check.

## Return Value

The tile map node object’s tile column index for the specified position.

## See Also

### Querying the Tile Map’s Properties

func centerOfTile(atColumn: Int, row: Int) -> CGPoint

func tileDefinition(atColumn: Int, row: Int) -> SKTileDefinition?

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

func tileRowIndex(fromPosition: CGPoint) -> Int

Returns the tile map node object’s tile row index for the specified position in points.

var mapSize: CGSize

The overall size of the tile map.

