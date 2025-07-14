

- RealityKit
-  ProjectiveTransformCameraComponent 

Structure

# ProjectiveTransformCameraComponent

A component that defines a virtual camera with a custom projection matrix.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ProjectiveTransformCameraComponent
```

## Overview

Each scene requires a camera, which defines the viewpoint from which RealityKit renders the scene. The projective transform camera renders the entities in the scene based on a custom user defined matrix. To create a projective transform camera, add this component to an entity.

```
// Create an entity to hold the camera component.
let cameraEntity = Entity()

// Create a projective transform camera component with a custom matrix.
var projectiveCameraComponent = ProjectiveTransformCameraComponent(projectionMatrix: customMatrix)

// Add it to the camera entity.
cameraEntity.components.set(projectiveCameraComponent)

// Set the entity's position and orientation to look at the subject.
let cameraPosition: SIMD3 = [0, 1, 3]

// The subject in this case is the origin.
let target: SIMD3 = .zero
cameraEntity.look(at: target, from: cameraPosition, relativeTo: nil)

// Add the camera entity to your scene.
content.add(cameraEntity)
```

## Topics

### Operators

static func == (ProjectiveTransformCameraComponent, ProjectiveTransformCameraComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(projectionMatrix: float4x4)

Creates a new custom matrix camera component with the given settings.

### Instance Properties

var transform: float4x4

The custom projection RealityKit applies to objects in the scene.

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

struct OrthographicCameraComponent

A component that defines an orthographic virtual camera and its settings.

enum CameraFieldOfViewOrientation

The orientations that a camera’s field-of-view degrees can apply.

class PerspectiveCamera

A virtual camera that establishes the rendering perspective.

