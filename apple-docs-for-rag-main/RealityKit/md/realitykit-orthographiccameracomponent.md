

- RealityKit
-  OrthographicCameraComponent 

Structure

# OrthographicCameraComponent

A component that defines an orthographic virtual camera and its settings.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct OrthographicCameraComponent
```

## Overview

Each scene requires a camera that defines the viewpoint from which RealityKit renders the scene. The orthographic camera renders the entities in the scene without the perspective of depth, meaning faraway objects don’t look smaller.

To create an orthographic camera, add this component to an entity.

| **Perspective camera** | **Orthographic camera** |
|----|----|
|  |  |

You can add an `OrthographicCameraComponent` to an entity’s component set, and orient that entity so that it looks at a specific target using look(at:from:upVector:relativeTo:).

```
// Create an entity to hold the camera component.
let cameraEntity = Entity()

// Create an orthographic camera component and add it to the camera entity.
cameraEntity.components.set(OrthographicCameraComponent())

// Set the entity's position and orientation to look at the subject.
let cameraPosition: SIMD3 = [0, 1, 3]

// The subject in this case is the origin.
let target: SIMD3 = .zero
cameraEntity.look(at: target, from: cameraPosition, relativeTo: nil)

// Add the camera entity to your scene.
content.add(cameraEntity)
```

In AR scenarios, the system provides the camera automatically; however, in non-AR scenarios, the app needs to set the camera. If the app doesn’t provide a camera, the system uses the default perspective camera.

## Topics

### Creating a camera component

init()

Creates an orthographic camera component with default values.

### Setting focal points

var far: Float

The maximum distance in meters from the camera that the camera can see.

var near: Float

The minimum distance in meters from the camera that the camera can see.

### Setting the camera scale

var scale: Float

A floating-point value the camera uses to scale entities.

var scaleDirection: CameraFieldOfViewOrientation

The direction in which the camera applies scaling.

### Comparing orthographic camera components

static func == (OrthographicCameraComponent, OrthographicCameraComponent) -> Bool

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

struct PerspectiveCameraComponent

A component that defines a virtual camera and its controls.

enum CameraFieldOfViewOrientation

The orientations that a camera’s field-of-view degrees can apply.

struct ProjectiveTransformCameraComponent

A component that defines a virtual camera with a custom projection matrix.

class PerspectiveCamera

A virtual camera that establishes the rendering perspective.

