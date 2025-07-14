

- SpriteKit
- SKTileDefinition
-  placementWeight 

Instance Property

# placementWeight

The placement weight of the tile definition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var placementWeight: Int { get set }
```

## Discussion

This value is used to determine how likely this tile definition is to be chosen for placement when a SKTileGroupRule has multiple tile definitions assigned to it. A higher value relative to the other definitions assigned to the rule make it more likely for this definition to be selected; lower values make it less likely. Defaults to 1. When set to 0, the definition will never be chosen as long as there is at least one other definition with a placementWeight above 0.

## See Also

### Reading or Adjusting a Tile’s Instance Properties

var name: String?

A name associated with the tile definition.

var size: CGSize

The size of the tile definition in points.

