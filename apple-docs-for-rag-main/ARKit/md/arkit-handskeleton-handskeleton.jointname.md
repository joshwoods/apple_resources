

- ARKit
- HandSkeleton
-  HandSkeleton.JointName 

Enumeration

# HandSkeleton.JointName

The names of different hand joints.

visionOS 1.0+

``` source
enum JointName
```

## Topics

### Forearm joints

case forearmArm

case forearmWrist

case wrist

### Thumb joints

case thumbIntermediateBase

case thumbIntermediateTip

case thumbKnuckle

case thumbTip

### Index finger joints

case indexFingerIntermediateBase

case indexFingerIntermediateTip

case indexFingerKnuckle

case indexFingerMetacarpal

case indexFingerTip

### Middle finger joints

case middleFingerIntermediateBase

case middleFingerIntermediateTip

case middleFingerKnuckle

case middleFingerMetacarpal

case middleFingerTip

### Ring finger joints

case ringFingerIntermediateBase

case ringFingerIntermediateTip

case ringFingerKnuckle

case ringFingerMetacarpal

case ringFingerTip

### Little finger joints

case littleFingerIntermediateBase

case littleFingerIntermediateTip

case littleFingerKnuckle

case littleFingerMetacarpal

case littleFingerTip

### Instance Properties

var description: String

A textual representation of this joint name.

## Relationships

### Conforms To

- CaseIterable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Retrieving specific hand joints

func joint(HandSkeleton.JointName) -> HandSkeleton.Joint

Retrieves a hand joint based on the joint name you specify.

struct Joint

The name and position of an individual hand joint.

