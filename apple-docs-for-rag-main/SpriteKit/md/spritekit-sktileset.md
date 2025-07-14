

- SpriteKit
-  SKTileSet 

Class

# SKTileSet

A container for related tile groups.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class SKTileSet
```

## Overview

An SKTileSet object contains an array of tile groups that define which tile definitions are available for use in a tile map.

Tile sets also define the arrangement of tiles within a tile map. In addition to the default rectangular grid layout, tile sets can also define hexagonal and isometric layouts.

## Topics

### Creating a Tile Set from a File

convenience init?(named: String)

Initializes a tile set by searching the app bundle for an archived `.sks` file by name.

convenience init?(from: URL)

Initializes a tile set from a URL to an archived .sks file.

### Creating a Tile Set Programmatically

Create a tile set by passing in the various groups that make up the set.

init(tileGroups: [SKTileGroup])

Initializes a new tile set with an array of tile groups and rectangular grid layout.

init(tileGroups: [SKTileGroup], tileSetType: SKTileSetType)

Initializes a new tile set with an array of tile groups and specified layout.

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

enum SKTileSetType

An enumeration defining how tiles are arranged.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Tiling

class SKTileMapNode

A two-dimensional array of images.

class SKTileDefinition

A single tile that can be repeated in a tile map.

class SKTileGroup

A set of tiles that collectively define one type of terrain.

class SKTileGroupRule

Rules that describe how various tiles should be placed in a map.

