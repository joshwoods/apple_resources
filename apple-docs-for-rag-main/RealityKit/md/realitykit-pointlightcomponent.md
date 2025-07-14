

- RealityKit
-  PointLightComponent 

Structure

# PointLightComponent

A component that defines a point light source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
struct PointLightComponent
```

## Overview

The strength of a point light depends on a combination of its intensity and attenuationRadius. The default values for these properties make this light comparable to high-power streetlights, or outdoor floodlights.

This table shows a few examples of common scenarios similar to a point light source:

| Scenario | Approximate lumens | Attenuation radius | Description |
|----|----|----|----|
| Candle flame | 10-15 lumens | ~1 meter | Very small light source |
| Nightlight | 20-30 lumens | 1-2 meters | Low-level lighting |
| 25W lightbulb | 200-300 lumens | 2-3 meters | Small room lighting |
| 40W lightbulb | 400-500 lumens | 3-4 meters | Moderate room lighting |
| 60W lightbulb | 700-800 lumens | 4-5 meters | General-purpose lighting |
| 100W lightbulb | 1,500-1,700 lumens | 5-6 meters | Bright room lighting |
| LED flashlight | 300-600 lumens | 50-70 meters | Long distance illumination |
| Car headlights (each, low-beam) | 700-1,200 lumens | 100-150 meters | Illuminates the road ahead |
| LED streetlight | 8,000-10,000 lumens | 20-30 meters | Illuminates large outdoor areas |
| Stadium lighting | ~100,000 lumens | 100-200 meters | Lights-up large outdoor areas |

Use this component by applying it to an entity’s components set. In this example, the light’s color is red:

```
let lightEntity = Entity()

let redLightComponent = PointLightComponent(color: .red)
lightEntity.components.set(redLightComponent)
```

The point light illuminates entities based on its distance from them. Here is a visual example of how a red `PointLightComponent` illuminates elements based on distance:

|  |  |  |
|----|----|----|

Note

The green dot in the above illustrations is only a visual representation of the light’s position.

## Topics

### Creating a point light component

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float)

Creates a point light component with a configuration.

init(cgColor: CGColor, intensity: Float, attenuationRadius: Float)

Creates a new instance with the specified color, intensity and attenuation.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

### Setting color

var color: PointLightComponent.Color

A color for the point light.

var color: PointLightComponent.Color

A color for the point light.

### Configuring the light

var attenuationRadius: Float

The distance from the light source where its intensity reaches zero.

var intensity: Float

The intensity of the point light, measured in lumen.

var attenuationFalloffExponent: Float

The exponent value for the light’s intensity falloff-transition curve.

### Registering a component type

static func registerComponent()

Registers a new component type.

### Comparing point light components

static func == (PointLightComponent, PointLightComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Supporting types

typealias Color

A platform-specific type used to define color for a point light.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

