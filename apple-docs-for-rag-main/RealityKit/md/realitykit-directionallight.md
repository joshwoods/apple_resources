

- RealityKit
-  DirectionalLight 

Class

# DirectionalLight

An entity that casts a virtual light in a particular direction.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
class DirectionalLight
```

## Overview

During an AR session, RealityKit automatically lights your virtual objects to match real-world lighting. You can also explicitly add virtual lights that act upon your virtual content. This is typically most useful outside of an AR session on iOS or macOS, where your RealityViewCameraContent camera property is set to virtual.

A directional light uniformly casts light along its local z-axis—specifically, along `[0, 0, -1]`. This is equivalent to creating an Entity, and then adding a DirectionalLightComponent to its components set. Use the light’s look(at:from:upVector:relativeTo:) method to aim the light in a particular direction.

You can configure the light’s color and intensity with the component properties in light. You can also control how or if it casts a shadow.

A RealityKit scene can contain up to eight dynamic lights, which are entities that contain a SpotLightComponent, PointLightComponent, or a DirectionalLightComponent. This limit doesn’t include light from image-based lighting.

## Topics

### Creating a directional light

init()

Creates a new entity.

### Configuring the directional light

var light: DirectionalLightComponent

A directional light component for the entity.

var shadow: DirectionalLightComponent.Shadow?

The shadow settings for a directional light.

### Default Implementations

HasDirectionalLight Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasDirectionalLight
- HasHierarchy
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

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

protocol HasDirectionalLight

An interface that defines a directional light source component.

