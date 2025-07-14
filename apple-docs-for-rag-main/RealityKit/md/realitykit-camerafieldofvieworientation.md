

- RealityKit
-  CameraFieldOfViewOrientation 

Enumeration

# CameraFieldOfViewOrientation

The orientations that a camera’s field-of-view degrees can apply.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum CameraFieldOfViewOrientation
```

## Topics

### Operators

static func == (CameraFieldOfViewOrientation, CameraFieldOfViewOrientation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case horizontal

Applies the field-of-view degrees in the camera’s horizontal axis.

case vertical

Applies the field-of-view degrees in the camera’s vertical axis.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Cameras

struct PerspectiveCameraComponent

A component that defines a virtual camera and its controls.

struct OrthographicCameraComponent

A component that defines an orthographic virtual camera and its settings.

struct ProjectiveTransformCameraComponent

A component that defines a virtual camera with a custom projection matrix.

class PerspectiveCamera

A virtual camera that establishes the rendering perspective.

