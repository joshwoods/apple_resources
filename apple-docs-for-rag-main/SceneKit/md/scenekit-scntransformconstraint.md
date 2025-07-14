

- SceneKit
-  SCNTransformConstraint 

Class

# SCNTransformConstraint

A constraint that runs a specified closure, block in Objective-C, to compute a new transform (position, rotation, and scale) for each node that the constraint affects.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNTransformConstraint
```

## Overview

To attach constraints to an SCNNode object, use its constraints property.

When Scene Kit prepares to render a scene, it evaluates the list of constraints attached to each node to determine the transformation for that node, then applies the new transformation before rendering. To evaluate a transform constraint, Scene Kit runs the block you provided when creating the constraint. In this block, your app computes a new transformation to be applied to the node. Optionally, your app may reference the node’s current transformation in computing the new transformation.

## Topics

### Creating a Transform Constraint

convenience init(inWorldSpace: Bool, with: (SCNNode, SCNMatrix4) -> SCNMatrix4)

Creates a new transform constraint.

### Type Methods

class func orientationConstraint(inWorldSpace: Bool, with: (SCNNode, SCNQuaternion) -> SCNQuaternion) -> Self

class func positionConstraint(inWorldSpace: Bool, with: (SCNNode, SCNVector3) -> SCNVector3) -> Self

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

