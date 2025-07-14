

- SpriteKit
- SKTileMapNode
-  setTileGroup(\_:andTileDefinition:forColumn:row:) 

Instance Method

# setTileGroup(\_:andTileDefinition:forColumn:row:)

Set the tile group and tile definition at the specified tile index.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func setTileGroup(
    _ tileGroup: SKTileGroup,
    andTileDefinition tileDefinition: SKTileDefinition,
    forColumn column: Int,
    row: Int
)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func setTileGroup(
    _ tileGroup: SKTileGroup,
    andTileDefinition tileDefinition: SKTileDefinition,
    forColumn column: Int,
    row: Int
)
```

## Parameters 

`tileGroup`  

The tile group to place in the map.

`tileDefinition`  

The tile definition to place in the map.

`column`  

The column index of the tile.

`row`  

The row index of the tile.

## Discussion

This function is for use when you’re creating a tile map programmatically, versus creating it ahead of time with the scene editor.

When enableAutomapping is set to `true`, the surrounding tiles of a painted area will be controlled by the tile group, too. When automapping is disabled, just the tile definition will be placed without modify any of the neighboring tiles.

## See Also

### Defining a Tile Map’s Contents

var enableAutomapping: Bool

When creating a tile map node programmatically, specifies whether the tile map uses automapping behavior like the scene editor.

func fill(with: SKTileGroup?)

When creating a tile map node programmatically, this function performs a fill operation with the specified tile group.

func setTileGroup(SKTileGroup?, forColumn: Int, row: Int)

Set the tile group at the specified tile index.

