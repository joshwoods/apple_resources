

- SceneKit
-  SCNAvoidOccluderConstraint 

Class

# SCNAvoidOccluderConstraint

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
class SCNAvoidOccluderConstraint
```

## Topics

### Creating a Constraint

convenience init(target: SCNNode?)

### Configuring Constraint Behavior

var bias: CGFloat

var occluderCategoryBitMask: Int

var target: SCNNode?

var delegate: any SCNAvoidOccluderConstraintDelegate

protocol SCNAvoidOccluderConstraintDelegate

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

### Position Constraints

class SCNDistanceConstraint

