

- RealityKit
-  HasDirectionalLight 

Protocol

# HasDirectionalLight

An interface that defines a directional light source component.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
protocol HasDirectionalLight : HasTransform
```

## Topics

### Getting the directional light

var light: DirectionalLightComponent

A directional light component for the entity.

### Specifying the shadow

var shadow: DirectionalLightComponent.Shadow?

The shadow settings for a directional light.

## Relationships

### Inherits From

- HasTransform

### Conforming Types

- DirectionalLight

## See Also

### Entity compliance

protocol HasPerspectiveCamera

An interface that enables you to configure a virtual camera that you can use to define the rendering perspective when you’re not in an AR session.

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

