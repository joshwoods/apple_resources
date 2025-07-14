

- SpriteKit
-  SKReachConstraints 

Class

# SKReachConstraints

A specification of the degree of freedom when solving inverse kinematics.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class SKReachConstraints
```

## Overview

An SKReachConstraints object is used to describe the range of motion for an SKNode object whenever an inverse kinematic (IK) action is executed. To use reach constraints, create an SKReachConstraints object and assign it to a node’s reachConstraints property. For more information on using reach actions to perform IK animations, see the SKAction class.

## Topics

### Working with Reach Constraints

init(lowerAngleLimit: CGFloat, upperAngleLimit: CGFloat)

Initializes a new reach constraint object.

var lowerAngleLimit: CGFloat

The minimum angle that the node can have after it is rotated by a reach event.

var upperAngleLimit: CGFloat

The maximum angle that the node can have after it is rotated by a reach event.

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
- NSObjectProtocol
- NSSecureCoding

## See Also

### Constraints

class SKConstraint

A specification for constraining a node’s position or rotation.

