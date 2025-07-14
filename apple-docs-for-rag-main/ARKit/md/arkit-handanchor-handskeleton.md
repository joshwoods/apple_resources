

- ARKit
- HandAnchor
-  handSkeleton 

Instance Property

# handSkeleton

The current position and orientation of joints on a hand.

visionOS 1.0+

``` source
var handSkeleton: HandSkeleton? { get }
```

## See Also

### Getting hand information

var originFromAnchorTransform: simd_float4x4

The location and orientation of a hand in world space.

var chirality: HandAnchor.Chirality

The chirality of this hand.

enum Chirality

A value that indicates a left or right hand.

var isTracked: Bool

A Boolean value that indicates whether ARKit is currently tracking this hand.

var description: String

A textual representation of this anchor.

