

- SceneKit
-  SCNBillboardConstraint 

Class

# SCNBillboardConstraint

A constraint that orients a node to always point toward the current camera.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class SCNBillboardConstraint
```

## Overview

An SCNBillboardConstraint object automatically adjusts a node’s orientation so that its local z-axis always points toward the pointOfView node currently being used to render the scene. For example, you can use a billboard constraint to efficiently render parts of a scene using two-dimensional sprite images instead of three-dimensional geometry—by mapping sprites onto planes affected by a billboard constraint, the sprites maintain their orientation with respect to the viewer. To attach constraints to an SCNNode object, use its constraints property.

## Topics

### Working with a Constraint’s Degrees of Freedom

var freeAxes: SCNBillboardAxis

An option that specifies which degrees of freedom the constraint affects.

### Constants

struct SCNBillboardAxis

Options for locking the orientation of nodes affected by a billboard constraint.

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

class SCNLookAtConstraint

A constraint that orients a node to always point toward a specified other node.

