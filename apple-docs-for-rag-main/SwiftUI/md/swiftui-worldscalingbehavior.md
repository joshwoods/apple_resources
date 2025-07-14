

- SwiftUI
-  WorldScalingBehavior 

Structure

# WorldScalingBehavior

Specifies the scaling behavior a window should have within the world.

visionOS 2.0+

``` source
struct WorldScalingBehavior
```

## Overview

By default, a regular WindowGroup uses a scaling behavior of dynamic, and a window with volumetric has a fixed scale.

Dynamic scale means the window will scale larger as it moves further away, maintaining the same angular size. Fixed scale means the window will keep its physical size in the world.

For further information, see Spatial layout in the Human Interface Guidelines.

## Topics

### Type Properties

static var automatic: WorldScalingBehavior

The scaling behavior that is standard for the window’s style.

static var dynamic: WorldScalingBehavior

The window will scale up as it moves further away, maintaining the same angular size.

## Relationships

### Conforms To

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

enum SquareAzimuth

A type describing what direction something is being viewed from along the horizontal plane and snapped to 4 directions.

struct WorldAlignmentBehavior

A type representing the world alignment behavior for a scene.

func volumeWorldAlignment(WorldAlignmentBehavior) -> some Scene

Specifies how a volume should be aligned when moved in the world.

func defaultWorldScaling(WorldScalingBehavior) -> some Scene

Specify the world scaling behavior for the window.

struct WorldScalingCompensation

Indicates whether returned metrics will take dynamic scaling into account.

var worldTrackingLimitations: Set&lt;WorldTrackingLimitation>

The current limitations of the device tracking the user’s surroundings.

struct WorldTrackingLimitation

A structure to represent limitations of tracking the user’s surroundings.

