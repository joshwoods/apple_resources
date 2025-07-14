

- Vision
-  Joint 

Structure

# Joint

A pose joint represented as a normalized point in an image, along with a label and a confidence value.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Joint
```

## Topics

### Inspecting a joint

let confidence: Float

A confidence score that indicates the detected joint’s accuracy.

let jointName: String

The joint’s identifier label.

let location: NormalizedPoint

The location of the joint in normalized coordinates.

### Getting the distance to a joint

func distance(to: Joint) -> CGFloat

Returns the distance to another joint.

## Relationships

### Conforms To

- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Body and hand pose detection

struct DetectHumanBodyPoseRequest

A request that detects a human body pose.

struct DetectHumanHandPoseRequest

A request that detects a human hand pose.

protocol PoseProviding

An observation that provides a collection of joints that make up a pose.

enum Chirality

The hand sidedness of a pose.

