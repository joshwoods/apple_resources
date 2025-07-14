

- Vision
- HumanHandPoseObservation
-  HumanHandPoseObservation.Chirality 

Enumeration

# HumanHandPoseObservation.Chirality

The hand sidedness of a pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Chirality
```

## Topics

### Getting the handedness

case left

case right

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting an observation

enum RequestDescriptor

A type that describes the request and revision combination.

let chirality: HumanHandPoseObservation.Chirality?

The chirality, or handedness, of a pose.

var keypoints: MLMultiArray

The keypoints for the observation.

