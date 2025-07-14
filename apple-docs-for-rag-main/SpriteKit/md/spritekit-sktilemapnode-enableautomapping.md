

- SpriteKit
- SKTileMapNode
-  enableAutomapping 

Instance Property

# enableAutomapping

When creating a tile map node programmatically, specifies whether the tile map uses automapping behavior like the scene editor.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**watchOS**

``` source
var enableAutomapping: Bool { get set }
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
var enableAutomapping: Bool { get set }
```

## Discussion

This function is for use when you’re creating a tile map programmatically, versus creating it ahead of time with the scene editor.

Set this value to `true` when you want automapping behavior (equivalent to using the paint brush in the scene editor) when using the fill(with:), and setTileGroup(_:andTileDefinition:forColumn:row:) functions.

## See Also

### Defining a Tile Map’s Contents

func fill(with: SKTileGroup?)

When creating a tile map node programmatically, this function performs a fill operation with the specified tile group.

func setTileGroup(SKTileGroup, andTileDefinition: SKTileDefinition, forColumn: Int, row: Int)

Set the tile group and tile definition at the specified tile index.

func setTileGroup(SKTileGroup?, forColumn: Int, row: Int)

Set the tile group at the specified tile index.

