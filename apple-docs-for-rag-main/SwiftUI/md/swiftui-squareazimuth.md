

- SwiftUI
-  SquareAzimuth 

Enumeration

# SquareAzimuth

A type describing what direction something is being viewed from along the horizontal plane and snapped to 4 directions.

visionOS 2.0+

``` source
@frozen
enum SquareAzimuth
```

## Topics

### Structures

struct Set

### Enumeration Cases

case back

Has an orientation with an horizontal angle equal to `180°`

case front

Has an orientation with an horizontal angle equal to `0°`.

case left

Has an orientation with an horizontal angle equal to `270°`.

case right

Has an orientation with an horizontal angle equal to `90°`.

### Initializers

init(closestToAzimuth: Angle)

Creates a SquareAzimuth case with an orientation that has a horizontal angle closest to the provided azimuth.

### Instance Properties

var orientation: Rotation3D

A 3D rotation that is snapped to the center of one of the four sides.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Interacting with volumes

func onVolumeViewpointChange(updateStrategy: VolumeViewpointUpdateStrategy, initial: Bool, (Viewpoint3D, Viewpoint3D) -> Void) -> some View

Adds an action to perform when the viewpoint of the volume changes.

func supportedVolumeViewpoints(SquareAzimuth.Set) -> some View

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

struct VolumeViewpointUpdateStrategy

A type describing when the action provided to onVolumeViewpointChange(updateStrategy:initial:_:) should be called.

struct Viewpoint3D

A type describing what direction something is being viewed from.

struct WorldAlignmentBehavior

A type representing the world alignment behavior for a scene.

func volumeWorldAlignment(WorldAlignmentBehavior) -> some Scene

Specifies how a volume should be aligned when moved in the world.

struct WorldScalingBehavior

Specifies the scaling behavior a window should have within the world.

func defaultWorldScaling(WorldScalingBehavior) -> some Scene

Specify the world scaling behavior for the window.

struct WorldScalingCompensation

Indicates whether returned metrics will take dynamic scaling into account.

var worldTrackingLimitations: Set&lt;WorldTrackingLimitation>

The current limitations of the device tracking the user’s surroundings.

struct WorldTrackingLimitation

A structure to represent limitations of tracking the user’s surroundings.

