

- SpriteKit
-  SKTileGroupRule 

Class

# SKTileGroupRule

Rules that describe how various tiles should be placed in a map.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
class SKTileGroupRule
```

## Overview

When a tile is filled in a tile map, the tile group rule defines how neighboring tiles are populated based on adjacency rules. A rule with multiple definitions uses the placement weights of the definitions to randomly select which to use.

## Topics

### Creating a Tile Group Rule

init(adjacency: SKTileAdjacencyMask, tileDefinitions: [SKTileDefinition])

Initializes a new tile group rule with adjacency rules and tile definitions.

### Accessing or Setting Tile Group Rule Properties

var adjacency: SKTileAdjacencyMask

The adjacency requirement for this rule.

struct SKTileAdjacencyMask

An enumeration defining how neighboring tiles are automatically placed next to each other.

var name: String?

A name associated with the tile group rule.

var tileDefinitions: [SKTileDefinition]

The tile definitions used for this rule.

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

class SKTileSet

A container for related tile groups.

