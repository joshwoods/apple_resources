

- SpriteKit
- SKTileMapNode
-  tileRowIndex(fromPosition:) 

Instance Method

# tileRowIndex(fromPosition:)

Returns the tile map node object’s tile row index for the specified position in points.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func tileRowIndex(fromPosition position: CGPoint) -> Int
```

**watchOS**

``` source
func tileRowIndex(fromPosition position: CGPoint) -> Int
```

## Parameters 

`position`  

The position in the tile map to check.

## Return Value

The tile map node object’s tile row index for the specified position.

## See Also

### Querying the Tile Map’s Properties

func centerOfTile(atColumn: Int, row: Int) -> CGPoint

func tileColumnIndex(fromPosition: CGPoint) -> Int

func tileDefinition(atColumn: Int, row: Int) -> SKTileDefinition?

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

var mapSize: CGSize

The overall size of the tile map.

