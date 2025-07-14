

- SpriteKit
-  SKTileAdjacencyMask 

Structure

# SKTileAdjacencyMask

An enumeration defining how neighboring tiles are automatically placed next to each other.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
struct SKTileAdjacencyMask
```

## Topics

### Initializers

init(rawValue: UInt)

### Masks

static var adjacencyAll: SKTileAdjacencyMask

static var adjacencyDown: SKTileAdjacencyMask

static var adjacencyDownEdge: SKTileAdjacencyMask

static var adjacencyLeft: SKTileAdjacencyMask

static var adjacencyLeftEdge: SKTileAdjacencyMask

static var adjacencyLowerLeft: SKTileAdjacencyMask

static var adjacencyLowerLeftCorner: SKTileAdjacencyMask

static var adjacencyLowerLeftEdge: SKTileAdjacencyMask

static var adjacencyLowerRight: SKTileAdjacencyMask

static var adjacencyLowerRightCorner: SKTileAdjacencyMask

static var adjacencyLowerRightEdge: SKTileAdjacencyMask

static var adjacencyRight: SKTileAdjacencyMask

static var adjacencyRightEdge: SKTileAdjacencyMask

static var adjacencyUp: SKTileAdjacencyMask

static var adjacencyUpEdge: SKTileAdjacencyMask

static var adjacencyUpperLeft: SKTileAdjacencyMask

static var adjacencyUpperLeftCorner: SKTileAdjacencyMask

static var adjacencyUpperLeftEdge: SKTileAdjacencyMask

static var adjacencyUpperRight: SKTileAdjacencyMask

static var adjacencyUpperRightCorner: SKTileAdjacencyMask

static var adjacencyUpperRightEdge: SKTileAdjacencyMask

static var hexFlatAdjacencyAll: SKTileAdjacencyMask

static var hexFlatAdjacencyDown: SKTileAdjacencyMask

static var hexFlatAdjacencyLowerLeft: SKTileAdjacencyMask

static var hexFlatAdjacencyLowerRight: SKTileAdjacencyMask

static var hexFlatAdjacencyUp: SKTileAdjacencyMask

static var hexFlatAdjacencyUpperLeft: SKTileAdjacencyMask

static var hexFlatAdjacencyUpperRight: SKTileAdjacencyMask

static var hexPointyAdjacencyAdd: SKTileAdjacencyMask

static var hexPointyAdjacencyLeft: SKTileAdjacencyMask

static var hexPointyAdjacencyLowerLeft: SKTileAdjacencyMask

static var hexPointyAdjacencyLowerRight: SKTileAdjacencyMask

static var hexPointyAdjacencyRight: SKTileAdjacencyMask

static var hexPointyAdjacencyUpperLeft: SKTileAdjacencyMask

static var hexPointyAdjacencyUpperRight: SKTileAdjacencyMask

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Accessing or Setting Tile Group Rule Properties

var adjacency: SKTileAdjacencyMask

The adjacency requirement for this rule.

var name: String?

A name associated with the tile group rule.

var tileDefinitions: [SKTileDefinition]

The tile definitions used for this rule.

