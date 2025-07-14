

- SwiftUI
-  VolumeViewpointUpdateStrategy 

Structure

# VolumeViewpointUpdateStrategy

A type describing when the action provided to onVolumeViewpointChange(updateStrategy:initial:_:) should be called.

visionOS 2.0+

``` source
struct VolumeViewpointUpdateStrategy
```

## Topics

### Type Properties

static let all: VolumeViewpointUpdateStrategy

The action should be run for all viewpoint changes.

static let supported: VolumeViewpointUpdateStrategy

The action should only be run when the new viewpoint is equivalent to one of the values provided through supportedVolumeViewpoints(_:).

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Interacting with volumes

func onVolumeViewpointChange(updateStrategy: VolumeViewpointUpdateStrategy, initial: Bool, (Viewpoint3D, Viewpoint3D) -> Void) -> some View

Adds an action to perform when the viewpoint of the volume changes.

func supportedVolumeViewpoints(SquareAzimuth.Set) -> some View

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

struct Viewpoint3D

A type describing what direction something is being viewed from.

enum SquareAzimuth

A type describing what direction something is being viewed from along the horizontal plane and snapped to 4 directions.

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

