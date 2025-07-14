

- SpriteKit
- SKTileGroupRule
-  tileDefinitions 

Instance Property

# tileDefinitions

The tile definitions used for this rule.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var tileDefinitions: [SKTileDefinition] { get set }
```

## Discussion

When this rule is evaluated and its conditions met, one of the definitions is randomly selected for placement based on their placement weights.

## See Also

### Accessing or Setting Tile Group Rule Properties

var adjacency: SKTileAdjacencyMask

The adjacency requirement for this rule.

struct SKTileAdjacencyMask

An enumeration defining how neighboring tiles are automatically placed next to each other.

var name: String?

A name associated with the tile group rule.

