

- SpriteKit
- SKTileMapNode
-  fill(with:) 

Instance Method

# fill(with:)

When creating a tile map node programmatically, this function performs a fill operation with the specified tile group.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
func fill(with tileGroup: SKTileGroup?)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func fill(with tileGroup: SKTileGroup?)
```

## Parameters 

`tileGroup`  

The tile group that will be used to fill the map.

## Mentioned in 

Creating Tile Groups Programmatically

## Discussion

This function is for use when you’re creating a tile map programmatically, versus creating it ahead of time with the scene editor.

## See Also

### Defining a Tile Map’s Contents

var enableAutomapping: Bool

When creating a tile map node programmatically, specifies whether the tile map uses automapping behavior like the scene editor.

func setTileGroup(SKTileGroup, andTileDefinition: SKTileDefinition, forColumn: Int, row: Int)

Set the tile group and tile definition at the specified tile index.

func setTileGroup(SKTileGroup?, forColumn: Int, row: Int)

Set the tile group at the specified tile index.

