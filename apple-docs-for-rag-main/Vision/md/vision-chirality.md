

- Vision
-  Chirality 

Enumeration

# Chirality

The hand sidedness of a pose.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum Chirality
```

## Topics

### Getting the hand sidedness

case left

A case that represents the left hand.

case right

A case that represents the right hand.

## Relationships

### Conforms To

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

struct Joint

A pose joint represented as a normalized point in an image, along with a label and a confidence value.

