

- SwiftUI
- EnvironmentValues
-  worldTrackingLimitations 

Instance Property

# worldTrackingLimitations

The current limitations of the device tracking the user’s surroundings.

visionOS 2.0+

``` source
var worldTrackingLimitations: Set { get set }
```

## Discussion

Read this environment value from within a view to obtain the current limitations of the device tracking the user’s surroundings. The device’s capabilities may be limited due to physical circumstances such as the lighting. If any of the limitations occur due to changing circumstances, the set is updated accordingly. For example, the following Text view automatically updates when the world tracking limitations change:

```
@Environment(\.worldTrackingLimitations)
private var worldTrackingLimitations

var body: some View {
    Text("Can track translation?" + worldTrackingLimitations
        .contains(.translation) ? "No" : "Yes")
}
```

When the device’s world tracking capabilities are limited, don’t prevent the user from experiencing your app entirely. Instead, try to adapt the user experience to the current circumstances in order to provide a meaningful experience at all times.

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

struct WorldScalingCompensation

Indicates whether returned metrics will take dynamic scaling into account.

struct WorldTrackingLimitation

A structure to represent limitations of tracking the user’s surroundings.

