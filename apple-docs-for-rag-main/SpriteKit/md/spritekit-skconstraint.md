

- SpriteKit
-  SKConstraint 

Class

# SKConstraint

A specification for constraining a node’s position or rotation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class SKConstraint
```

## Mentioned in 

Working with Inverse Kinematics

## Overview

An SKConstraint object describes a mathematical constraint on a node’s position or orientation. You attach constraints to nodes; after a scene processes any actions and physics interactions, it applies constraints attached to nodes in its node tree. Use constraints to ensure that certain relationships are true before the system renders a scene. For example, you might use a constraint to:

- Change a node’s zRotation property so that it always points at another node or a position in the scene.

- Keep a node within a specified distance of another node or a point in the scene.

- Keep a node inside a specified rectangle.

- Restrict the zRotation property of a node so that it has a more limited rotation range of motion.

To use constraints, create an NSArray object that contains one or more constraint objects and assign the array to a node’s constraints property. When the system evaluates a scene, it executes the constraints on a node in the order they appear in the constraints array.

You can’t change a constraint after you create it. However, you can selectively disable or enable a constraint by setting its enabled property. You can also use the referenceNode property to convert positions to the referenced coordinate system before applying the constraint.

## Topics

### Creating Position Constraints

Limit a node’s movement in one axis or both.

Creating Position Constraints

Create a position constraint and add it to a node.

class func positionX(SKRange, y: SKRange) -> Self

Creates a constraint that restricts both coordinates of a node’s position.

class func positionX(SKRange) -> Self

Creates a constraint that restricts the x-coordinate of a node’s position.

class func positionY(SKRange) -> Self

Creates a constraint that restricts the y-coordinate of a node’s position.

### Creating Orientation Constraints

Provide limitations on a node’s rotation, or create rules the system uses to update a node’s rotation for you.

Creating a Look-At Constraint

Make a node automatically rotate itself based on the changing position of another node, by using orientation constraints.

class func orient(to: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face another node.

class func orient(to: CGPoint, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a fixed point.

class func orient(to: CGPoint, in: SKNode, offset: SKRange) -> Self

Creates a constraint that forces a node to rotate to face a point in another node’s coordinate system.

class func zRotation(SKRange) -> Self

Creates a constraint that limits the orientation of a node.

### Creating Distance Constraints

Create a rule the system uses to update a node’s position relative to another node in the scene.

class func distance(SKRange, to: SKNode) -> Self

Creates a constraint that keeps a node within a certain distance of another node.

class func distance(SKRange, to: CGPoint) -> Self

Creates a constraint that keeps a node within a certain distance of a point.

class func distance(SKRange, to: CGPoint, in: SKNode) -> Self

Creates a constraint that keeps a node within a certain distance of a point in another node’s coordinate system.

### Controlling the Coordinate System Where a Constraint is Applied

var referenceNode: SKNode?

The node whose coordinate system should be used to apply the constraint.

### Enabling and Disabling a Constraint

var enabled: Bool

A Boolean value that specifies whether the constraint is applied.

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

### Constraints

class SKReachConstraints

A specification of the degree of freedom when solving inverse kinematics.

