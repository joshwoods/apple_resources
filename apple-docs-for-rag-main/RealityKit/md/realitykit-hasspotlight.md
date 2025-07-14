

- RealityKit
-  HasSpotLight 

Protocol

# HasSpotLight

An interface that defines a spot light source component.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
protocol HasSpotLight : HasTransform
```

## Topics

### Getting the spot light

var light: SpotLightComponent

A spotlight component for the entity.

### Specifying the shadow

var shadow: SpotLightComponent.Shadow?

The shadow for the spotlight.

## Relationships

### Inherits From

- HasTransform

### Conforming Types

- SpotLight

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

class DirectionalLight

An entity that casts a virtual light in a particular direction.

protocol HasDirectionalLight

An interface that defines a directional light source component.

