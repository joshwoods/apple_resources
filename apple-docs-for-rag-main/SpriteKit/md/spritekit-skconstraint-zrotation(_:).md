

- SpriteKit
- SKConstraint
-  zRotation(\_:) 

Type Method

# zRotation(\_:)

Creates a constraint that limits the orientation of a node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func zRotation(_ zRange: SKRange) -> Self
```

## Parameters 

`zRange`  

A range value that specifies the minimum and maximum values of the node’s zRotation property.

## Return Value

A new constraint.

## Mentioned in 

Creating a Look-At Constraint

## Discussion

Each time when constraints are applied, the node’s zRotation property is clamped so that it is within the specified range.

## See Also

### Creating Orientation Constraints

Creating a Look-At Constraint

Make a node automatically rotate itself based on the changing position of another node, by using orientation constraints.

class func orient(to: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face another node.

class func orient(to: CGPoint, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a fixed point.

class func orient(to: CGPoint, in: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a point in another node’s coordinate system.

