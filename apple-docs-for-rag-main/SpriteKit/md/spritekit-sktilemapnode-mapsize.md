

- SpriteKit
- SKTileMapNode
-  mapSize 

Instance Property

# mapSize

The overall size of the tile map.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
var mapSize: CGSize { get }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var mapSize: CGSize { get }
```

## Discussion

For a grid set type, the overall size, in points, of the node will be numberOfColumns `*` tileSize `.` width wide and numberOfRows `*` tileSize `.` height high.

## See Also

### Querying the Tile Map’s Properties

func centerOfTile(atColumn: Int, row: Int) -> CGPoint

func tileColumnIndex(fromPosition: CGPoint) -> Int

func tileDefinition(atColumn: Int, row: Int) -> SKTileDefinition?

func tileGroup(atColumn: Int, row: Int) -> SKTileGroup?

func tileRowIndex(fromPosition: CGPoint) -> Int

Returns the tile map node object’s tile row index for the specified position in points.

