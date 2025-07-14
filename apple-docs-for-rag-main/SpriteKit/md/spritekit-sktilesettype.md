

- SpriteKit
-  SKTileSetType 

Enumeration

# SKTileSetType

An enumeration defining how tiles are arranged.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
enum SKTileSetType
```

## Topics

### Enumeration Cases

case grid

case hexagonalFlat

case hexagonalPointy

case isometric

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing or Reading a Tile Set’s Properties

var defaultTileGroup: SKTileGroup?

The tile set’s default tile group.

var defaultTileSize: CGSize

The tile set’s default tile size.

var name: String?

A name associated with the tile set.

var tileGroups: [SKTileGroup]

The tile set’s array of tile group objects.

var type: SKTileSetType

The tile set’s type.

