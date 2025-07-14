

- RealityKit
-  PointLight 

Class

# PointLight

An entity that produces an omnidirectional light for virtual objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
@MainActor @preconcurrency
class PointLight
```

## Overview

During an AR session, RealityKit automatically lights your virtual objects to match real-world lighting. You can also explicitly add virtual lights that act upon your virtual content. This is typically most useful outside of an AR session on iOS or macOS, where your RealityViewCameraContent camera property is set to virtual.

The point light is an omnidirectional light that illuminates all the virtual content within a configurable radius from the light. This is equivalent to creating an Entity, and then adding a PointLightComponent to its components set.

A RealityKit scene can contain up to eight dynamic lights, which are entities that contain a SpotLightComponent, PointLightComponent, or a DirectionalLightComponent. This limit doesn’t include light from image-based lighting.

## Topics

### Creating a point light

init()

Creates a new entity.

### Configuring the point light

var light: PointLightComponent

A point light component for the entity.

### Default Implementations

HasPointLight Implementations

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasHierarchy
- HasPointLight
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

