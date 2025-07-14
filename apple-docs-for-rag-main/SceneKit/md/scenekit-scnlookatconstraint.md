

- SceneKit
-  SCNLookAtConstraint 

Class

# SCNLookAtConstraint

A constraint that orients a node to always point toward a specified other node.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNLookAtConstraint
```

## Overview

For example, you can use a look-at constraint to ensure that a camera or spotlight always follows the movement of a game character. To attach constraints to an SCNNode object, use its constraints property.

A node points in the direction of the negative z-axis of its local coordinate system. This axis defines the view direction for nodes containing cameras and the lighting direction for nodes containing spotlights or directional lights, as well as the orientation of the node’s geometry and child nodes. When Scene Kit evaluates a look-at constraint, it updates the constrained node’s transform property so that the node’s negative z-axis points toward the constraint’s target node.

## Topics

### Creating a Look-At Constraint

convenience init(target: SCNNode?)

Creates a look-at constraint for a specified target node.

### Modifying a Constraint

var isGimbalLockEnabled: Bool

A Boolean value that specifies whether constrained nodes are allowed to rotate.

var target: SCNNode?

The node toward which constrained nodes will point after being reoriented.

### Instance Properties

var localFront: SCNVector3

var targetOffset: SCNVector3

var worldUp: SCNVector3

## Relationships

### Inherits From

- SCNConstraint

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
- SCNAnimatable

## See Also

### Orientation Constraints

class SCNBillboardConstraint

A constraint that orients a node to always point toward the current camera.

