

- RealityKit
-  HasPerspectiveCamera 

Protocol

# HasPerspectiveCamera

An interface that enables you to configure a virtual camera that you can use to define the rendering perspective when you’re not in an AR session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
protocol HasPerspectiveCamera : HasTransform
```

## Topics

### Getting the camera

var camera: PerspectiveCameraComponent

A camera component for the perspective camera entity.

## Relationships

### Inherits From

- HasTransform

### Conforming Types

- PerspectiveCamera

## See Also

### Entity compliance

class PointLight

An entity that produces an omnidirectional light for virtual objects.

protocol HasPointLight

An interface that defines a point light source component.

class SpotLight

An entity that illuminates virtual content in a cone-shaped volume.

protocol HasSpotLight

An interface that defines a spot light source component.

class DirectionalLight

An entity that casts a virtual light in a particular direction.

protocol HasDirectionalLight

An interface that defines a directional light source component.

