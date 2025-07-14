

- ARKit
-  HandSkeleton 

Structure

# HandSkeleton

A collection of joints in a hand.

visionOS 1.0+

``` source
struct HandSkeleton
```

## Topics

### Retrieving specific hand joints

func joint(HandSkeleton.JointName) -> HandSkeleton.Joint

Retrieves a hand joint based on the joint name you specify.

struct Joint

The name and position of an individual hand joint.

enum JointName

The names of different hand joints.

### Inspecting hand skeletons

var allJoints: [HandSkeleton.Joint]

All of the joints in a hand skeleton.

static var neutralPose: HandSkeleton

A hand pose that you can use as a reference.

var description: String

A textual representation of this Skeleton.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Hand tracking

Happy Beam

Leverage a Full Space to create a fun game using ARKit.

class HandTrackingProvider

A source of live data about the position of a person’s hands and hand joints.

struct HandAnchor

A hand’s position in a person’s surroundings.

