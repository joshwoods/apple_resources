

- SceneKit
-  SCNAvoidOccluderConstraintDelegate 

Protocol

# SCNAvoidOccluderConstraintDelegate

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
protocol SCNAvoidOccluderConstraintDelegate : NSObjectProtocol
```

## Topics

### Instance Methods

func avoidOccluderConstraint(SCNAvoidOccluderConstraint, didAvoidOccluder: SCNNode, for: SCNNode)

func avoidOccluderConstraint(SCNAvoidOccluderConstraint, shouldAvoidOccluder: SCNNode, for: SCNNode) -> Bool

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Configuring Constraint Behavior

var bias: CGFloat

var occluderCategoryBitMask: Int

var target: SCNNode?

var delegate: any SCNAvoidOccluderConstraintDelegate

