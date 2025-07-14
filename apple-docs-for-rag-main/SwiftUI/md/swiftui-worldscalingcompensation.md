

- SwiftUI
-  WorldScalingCompensation 

Structure

# WorldScalingCompensation

Indicates whether returned metrics will take dynamic scaling into account.

visionOS 2.0+

``` source
struct WorldScalingCompensation
```

## Overview

On visionOS, a window scene or a volume scene with the defaultWorldScaling(_:) modifier may scale dynamically when the user repositions it. In those cases, the metrics returned by a PhysicalMetric or PhysicalMetricsConverter value may or may not correspond to the units of a `RealityView`.

World scale compensation lets you specify if this scaling is taken into account. If the values are unscaled, they will correspond to the physical metrics of the user’s surroundings, regardless of dynamic scale. If scaled, they will be scaled appropriately for the scene, which means they will match the default coordinate system of a `RealityView` in that scene.

## Topics

### Type Properties

static let scaled: WorldScalingCompensation

Returns metrics that are scaled appropriately to match the coordinate system of their scene, including any world scaling behavior.

static let unscaled: WorldScalingCompensation

Returns metrics that match the scale of the user’s surroundings, regardless of the world scaling behavior of their scene.

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

struct WorldScalingBehavior

Specifies the scaling behavior a window should have within the world.

func defaultWorldScaling(WorldScalingBehavior) -> some Scene

Specify the world scaling behavior for the window.

var worldTrackingLimitations: Set&lt;WorldTrackingLimitation>

The current limitations of the device tracking the user’s surroundings.

struct WorldTrackingLimitation

A structure to represent limitations of tracking the user’s surroundings.

