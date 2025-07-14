

- SpriteKit
- SKConstraint
-  orient(to:offset:) 

Type Method

# orient(to:offset:)

Creates a constraint that forces a node to rotate to face another node.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func orient(
    to node: SKNode,
    offset radians: SKRange
) -> Self
```

## Parameters 

`node`  

The node that should be used to orient the node that this constraint is attached to.

`radians`  

An offset that is added to the zRotation value after it is calculated.

## Return Value

A new constraint.

## Discussion

Each time when constraints are applied, a new angle is calculated so that a line projected at this angle would point at the other node’s origin. This angle is added to the values specified in the `radians` property to create a new range. Finally, the node’s zRotation value is clamped to fit inside this range.

## See Also

### Creating Orientation Constraints

Creating a Look-At Constraint

Make a node automatically rotate itself based on the changing position of another node, by using orientation constraints.

class func orient(to: CGPoint, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a fixed point.

class func orient(to: CGPoint, in: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a point in another node’s coordinate system.

class func zRotation(SKRange) -> Self

Creates a constraint that limits the orientation of a node.

