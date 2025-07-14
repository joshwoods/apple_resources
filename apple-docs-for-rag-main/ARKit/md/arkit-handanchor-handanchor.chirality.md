

- ARKit
- HandAnchor
-  HandAnchor.Chirality 

Enumeration

# HandAnchor.Chirality

A value that indicates a left or right hand.

visionOS 1.0+

``` source
@frozen
enum Chirality
```

## Topics

### Getting hand chirality

case left

A left hand.

case right

A right hand.

### Instance Properties

var description: String

A textual representation of HandAnchor.Chirality

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting hand information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a hand in world space.

var handSkeleton: HandSkeleton?

The current position and orientation of joints on a hand.

var chirality: HandAnchor.Chirality

The chirality of this hand.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this hand.

var description: String

A textual representation of this anchor.

