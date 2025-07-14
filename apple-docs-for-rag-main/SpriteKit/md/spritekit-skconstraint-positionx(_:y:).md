

- SpriteKit
- SKConstraint
-  positionX(\_:y:) 

Type Method

# positionX(\_:y:)

Creates a constraint that restricts both coordinates of a node’s position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func positionX(
    _ xRange: SKRange,
    y yRange: SKRange
) -> Self
```

## Parameters 

`xRange`  

The range to restrict the x-coordinate to.

`yRange`  

The range to restrict the y-coordinate to.

## Return Value

A new constraint.

## Mentioned in 

Creating Position Constraints

## Discussion

Each time constraints are applied, the node’s position property is clamped so that both coordinates lie inside the specified ranges.

## See Also

### Creating Position Constraints

Creating Position Constraints

Create a position constraint and add it to a node.

class func positionX(SKRange) -> Self

Creates a constraint that restricts the x-coordinate of a node’s position.

class func positionY(SKRange) -> Self

Creates a constraint that restricts the y-coordinate of a node’s position.

