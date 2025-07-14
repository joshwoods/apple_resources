

- RealityKit
-  DirectionalLightComponent 

Structure

# DirectionalLightComponent

A component that defines a directional light source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
struct DirectionalLightComponent
```

## Overview

A directional light shines in the entity’s forward direction `[0, 0, -1]`.

Change the a directional light’s direction with the orientation or look(at:from:upVector:relativeTo:) method of the Entity with a `DirectionalLightComponent`. The position of the entity does not play a part in the directional light’s effect.

Tip

Turn on shadows for a directional light by adding the DirectionalLightComponent.Shadow component to an entity that has a `DirectionalLightComponent`.

Use this component with shadows by adding `DirectionalLightComponent` and DirectionalLightComponent.Shadow to an entity’s components set. In this example, the light’s color is red, and the intensity is `10_000`, which is an approximate lux for ambient daylight:

```
let lightEntity = Entity()

let redLightComponent = DirectionalLightComponent(
    color: .red, intensity: 10_000
)
let lightShadowComponent = DirectionalLightComponent.Shadow()
lightEntity.components.set([redLightComponent, lightShadowComponent])
```

The directional light illuminates entities evenly in the direction it derives from the orientation of `lightEntity`. Here is a visual example of how the above code snippet could illuminates entities in a scene:

| Without a directional light | With a directional light |
|----|----|
|  |  |

Note

The green arrows in the above illustration are only a visual representation of the light’s direction.

## Topics

### Creating a directional light

init(color: DirectionalLightComponent.Color, intensity: Float)

Creates a directional light with a configuration.

init(color: DirectionalLightComponent.Color, intensity: Float, isRealWorldProxy: Bool)

Creates a directional light with a configuration.

init(color: DirectionalLightComponent.Color, intensity: Float, isRealWorldProxy: Bool)

Creates a directional light with a configuration.

### Setting the color

var color: DirectionalLightComponent.Color

A color for the directional light.

var color: DirectionalLightComponent.Color

A color for the directional light.

### Setting intensity and shadows

var intensity: Float

The intensity of the directional light, measured in lumen per square meter.

var isRealWorldProxy: Bool

A Boolean that you use to control whether the directional light operates as a proxy for a real-world light.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing directional light components

static func == (DirectionalLightComponent, DirectionalLightComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Supporting types

typealias Color

A platform-specific type used to define color for a directional light.

### Structures

struct Shadow

A directional light component that adds shadows to entities that it illuminates

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Directional lights and their shadows

struct Shadow

A directional light component that adds shadows to entities that it illuminates

enum ShadowProjectionType

typealias ShadowMapCullMode

