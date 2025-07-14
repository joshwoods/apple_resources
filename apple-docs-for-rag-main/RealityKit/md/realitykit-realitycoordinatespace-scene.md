

- RealityKit
- RealityCoordinateSpace
-  scene 

Type Property

# scene

The coordinate space that represents ARKit world space.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
static var scene: SceneRealityCoordinateSpace { get }
```

Available when `Self` is `SceneRealityCoordinateSpace`.

## Discussion

In a visionOS window or volume, or when using the virtual camera on any other platform, this space represents the center of the scene’s owning RealityView.

When in a visionOS Immersive Space, or using the `RealityViewCamera/worldTracking` camera in iOS, the `scene` coordinate space is the ARKit world origin.

Note

This static type is equivalent to a SceneRealityCoordinateSpace instance.

