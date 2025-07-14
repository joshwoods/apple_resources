

- SpriteKit
- SKConstraint
-  orient(to:in:offset:) 

Type Method

# orient(to:in:offset:)

Creates a constraint that forces a node to rotate to face a point in another node’s coordinate system.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func orient(
    to point: CGPoint,
    in node: SKNode,
    offset radians: SKRange
) -> Self
```

## Parameters 

`point`  

A point in the `node` parameter’s coordinate system.

`node`  

The node whose coordinate system the point is specified in.

`radians`  

An offset that is added to the zRotation value after it is calculated.

## Return Value

A new constraint.

## Discussion

Each time when constraints are applied, a new angle is calculated so that a line projected at this angle would point at the target point. This angle is added to the values specified in the `radians` property to create a new range. Finally, the node’s zRotation value is clamped to fit inside this range.

## See Also

### Creating Orientation Constraints

Creating a Look-At Constraint

Make a node automatically rotate itself based on the changing position of another node, by using orientation constraints.

class func orient(to: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face another node.

class func orient(to: CGPoint, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a fixed point.

class func zRotation(SKRange) -> Self

Creates a constraint that limits the orientation of a node.

