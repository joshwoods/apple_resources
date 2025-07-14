

- SwiftUI
-  Viewpoint3D 

Structure

# Viewpoint3D

A type describing what direction something is being viewed from.

visionOS 2.0+

``` source
struct Viewpoint3D
```

## Topics

### Instance Properties

var squareAzimuth: SquareAzimuth

A value describing what direction something is being viewed from along the horizontal plane.

### Type Properties

static let standard: Viewpoint3D

A value that represents being viewed from the front middle.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Interacting with volumes

func onVolumeViewpointChange(updateStrategy: VolumeViewpointUpdateStrategy, initial: Bool, (Viewpoint3D, Viewpoint3D) -> Void) -> some View

Adds an action to perform when the viewpoint of the volume changes.

func supportedVolumeViewpoints(SquareAzimuth.Set) -> some View

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

struct VolumeViewpointUpdateStrategy

A type describing when the action provided to onVolumeViewpointChange(updateStrategy:initial:_:) should be called.

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

