

- SwiftUI
-  WorldAlignmentBehavior 

Structure

# WorldAlignmentBehavior

A type representing the world alignment behavior for a scene.

visionOS 2.0+

``` source
struct WorldAlignmentBehavior
```

## Overview

A value of this type can be provided to the volumeWorldAlignment(_:) scene modifier to control the world alignment volumes should maintain as they are repositioned. The default value is automatic.

## Topics

### Type Properties

static var adaptive: WorldAlignmentBehavior

When lifted above eye level, the volume will tilt so the front remains fully visible.

static var automatic: WorldAlignmentBehavior

The world alignment behavior that is standard for the system.

static var gravityAligned: WorldAlignmentBehavior

The volume will not tilt so as to remain aligned with gravity.

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

struct VolumeViewpointUpdateStrategy

A type describing when the action provided to onVolumeViewpointChange(updateStrategy:initial:_:) should be called.

struct Viewpoint3D

A type describing what direction something is being viewed from.

enum SquareAzimuth

A type describing what direction something is being viewed from along the horizontal plane and snapped to 4 directions.

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

