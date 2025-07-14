

- SceneKit
-  SCNConstraint 

Class

# SCNConstraint

The abstract superclass for objects that automatically adjust the position, rotation, or scale of a node based on specified rules.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
class SCNConstraint
```

## Overview

To control the transform (position, rotation, and scale) of one or more SCNNode objects with constraints, create and configure instances of the SCNConstraint subclass that provides the behavior you want, then add those constraint objects to each node’s constraints array.

When SceneKit prepares to render a scene, it examines the list of constraints attached to each node to determine the transform for that node, then applies the new transformation before displaying the scene.

## Topics

### Tuning a Constraint’s Effect on Nodes

var influenceFactor: CGFloat

The influence of the constraint on the node’s transformation.

### Instance Properties

var isEnabled: Bool

var isIncremental: Bool

## Relationships

### Inherits From

- NSObject

### Inherited By

- SCNAccelerationConstraint
- SCNAvoidOccluderConstraint
- SCNBillboardConstraint
- SCNDistanceConstraint
- SCNIKConstraint
- SCNLookAtConstraint
- SCNReplicatorConstraint
- SCNSliderConstraint
- SCNTransformConstraint

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

