

- ARKit
-  HandAnchor 

Structure

# HandAnchor

A hand’s position in a person’s surroundings.

visionOS 1.0+

``` source
struct HandAnchor
```

## Topics

### Getting hand information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a hand in world space.

var handSkeleton: HandSkeleton?

The current position and orientation of joints on a hand.

var chirality: HandAnchor.Chirality

The chirality of this hand.

enum Chirality

A value that indicates a left or right hand.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this hand.

var description: String

A textual representation of this anchor.

### Identifying hand anchors

var id: UUID

The unique identifier of this anchor.

## Relationships

### Conforms To

- Anchor
- Copyable
- CustomStringConvertible
- Equatable
- Identifiable
- Sendable
- TrackableAnchor

## See Also

### Hand tracking

Happy Beam

Leverage a Full Space to create a fun game using ARKit.

class HandTrackingProvider

A source of live data about the position of a person’s hands and hand joints.

struct HandSkeleton

A collection of joints in a hand.

