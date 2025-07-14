

- SpriteKit
- SKTileSet
-  defaultTileGroup 

Instance Property

# defaultTileGroup

The tile set’s default tile group.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var defaultTileGroup: SKTileGroup? { get set }
```

## Discussion

With auto-mapping enabled, it is possible for some tiles to be removed because there is either no valid rule or a missing tile group for the required adjacency rule. In this situation, those tiles are replaced by the tile group specified by defaultTileGroup.

## See Also

### Accessing or Reading a Tile Set’s Properties

var defaultTileSize: CGSize

The tile set’s default tile size.

var name: String?

A name associated with the tile set.

var tileGroups: [SKTileGroup]

The tile set’s array of tile group objects.

var type: SKTileSetType

The tile set’s type.

enum SKTileSetType

An enumeration defining how tiles are arranged.

