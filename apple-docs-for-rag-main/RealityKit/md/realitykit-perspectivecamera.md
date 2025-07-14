

- RealityKit
-  PerspectiveCamera 

Class

# PerspectiveCamera

A virtual camera that establishes the rendering perspective.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
class PerspectiveCamera
```

## Overview

During an AR session, RealityKit automatically uses the device’s camera to define the perspective from which to render the scene. When rendering a scene outside of an AR session (with the view’s cameraMode property set to ARView.CameraMode.nonAR), RealityKit uses a PerspectiveCamera instead. You can add a perspective camera anywhere in your scene to control the point of view. If you don’t explicitly provide one, RealityKit creates a default camera for you.

## Topics

### Creating a camera

init()

Creates a perspective camera entity.

### Configuring the camera

var camera: PerspectiveCameraComponent

A camera component for the perspective camera entity.

### Default Implementations

HasPerspectiveCamera Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasHierarchy
- HasPerspectiveCamera
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### Cameras

struct PerspectiveCameraComponent

A component that defines a virtual camera and its controls.

struct OrthographicCameraComponent

A component that defines an orthographic virtual camera and its settings.

enum CameraFieldOfViewOrientation

The orientations that a camera’s field-of-view degrees can apply.

struct ProjectiveTransformCameraComponent

A component that defines a virtual camera with a custom projection matrix.

