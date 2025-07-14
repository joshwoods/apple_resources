

- RealityKit
-  PerspectiveCameraComponent 

Structure

# PerspectiveCameraComponent

A component that defines a virtual camera and its controls.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
struct PerspectiveCameraComponent
```

## Overview

Each scene requires a camera that defines the viewpoint from which RealityKit renders the scene. In RealityKit, the default camera is a *perspective camera*, which simulates the way real cameras and human vision work. Entities that are farther away from the camera render smaller.

For an alternative camera solution, see OrthographicCameraComponent.

To create a perspective camera, add this component to an entity.

```
let cameraEntity = Entity()

// Place the camera 2 meters along the z-axis,
// looking at the scene origin.
let cameraPosition: SIMD3 = [0, 0, 2]
cameraEntity.look(at: .zero, from: cameraPosition, relativeTo: nil)

cameraEntity.components.set(PerspectiveCameraComponent())
```

A `PerspectiveCameraComponent` defines the camera settings for a perspective camera, such as the fieldOfViewInDegrees. The entity’s transform defines the camera entity’s viewpoint and direction. The direction it points is along the entity’s negative z-axis.

In AR scenarios, the system provides the camera automatically; however, in non-AR scenarios, the app needs to set the camera. If the app doesn’t provide a camera, the system uses the default perspective camera.

## Topics

### Creating a camera component

init(near: Float, far: Float, fieldOfViewInDegrees: Float)

Creates a perspective camera component from near and far clipping planes and a field of view.

init(near: Float, far: Float, fieldOfViewInDegrees: Float, fieldOfViewOrientation: CameraFieldOfViewOrientation)

Creates a perspective camera component from near and far clipping planes, a field of view, and an orientation.

### Setting focal points

var far: Float

The maximum distance in meters from the camera that the camera can see.

var near: Float

The minimum distance in meters from the camera that the camera can see.

### Setting the field of view

var fieldOfViewInDegrees: Float

The camera’s total field of view in degrees.

var fieldOfViewOrientation: CameraFieldOfViewOrientation

The orientation with which the system uses to apply the field-of-view degrees.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing perspective camera components

static func == (PerspectiveCameraComponent, PerspectiveCameraComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Cameras

struct OrthographicCameraComponent

A component that defines an orthographic virtual camera and its settings.

enum CameraFieldOfViewOrientation

The orientations that a camera’s field-of-view degrees can apply.

struct ProjectiveTransformCameraComponent

A component that defines a virtual camera with a custom projection matrix.

class PerspectiveCamera

A virtual camera that establishes the rendering perspective.

