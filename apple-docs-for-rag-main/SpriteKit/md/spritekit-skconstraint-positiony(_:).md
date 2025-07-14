

- SpriteKit
- SKConstraint
-  positionY(\_:) 

Type Method

# positionY(\_:)

Creates a constraint that restricts the y-coordinate of a node’s position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func positionY(_ range: SKRange) -> Self
```

## Parameters 

`range`  

The range to restrict the coordinate to.

## Return Value

A new constraint.

## Mentioned in 

Creating Position Constraints

## Discussion

Each time when constraints are applied, the y-coordinate of the node’s position property is clamped so that it lies inside the specified range.

## See Also

### Creating Position Constraints

Creating Position Constraints

Create a position constraint and add it to a node.

class func positionX(SKRange, y: SKRange) -> Self

Creates a constraint that restricts both coordinates of a node’s position.

class func positionX(SKRange) -> Self

Creates a constraint that restricts the x-coordinate of a node’s position.

