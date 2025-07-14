

- SpriteKit
- SKTileSet
-  init(tileGroups:tileSetType:) 

Initializer

# init(tileGroups:tileSetType:)

Initializes a new tile set with an array of tile groups and specified layout.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
init(
    tileGroups: [SKTileGroup],
    tileSetType: SKTileSetType
)
```

## Parameters 

`tileGroups`  

An array of SKTileGroup objects from which to create the tile set from.

`tileSetType`  

The arrangement of the tiles.

## Return Value

A new tile set.

## See Also

### Creating a Tile Set Programmatically

init(tileGroups: [SKTileGroup])

Initializes a new tile set with an array of tile groups and rectangular grid layout.

