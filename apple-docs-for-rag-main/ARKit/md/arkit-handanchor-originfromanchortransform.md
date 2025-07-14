

- ARKit
- HandAnchor
-  originFromAnchorTransform 

Instance Property

# originFromAnchorTransform

The location and orientation of a hand in world space.

visionOS 1.0+

``` source
var originFromAnchorTransform: simd_float4x4 { get }
```

## Discussion

The transform of a hand anchor is positioned at the base of the wrist. ARKit provides transforms of other joints on the hand relative to this root transform.

## See Also

### Getting hand information

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

