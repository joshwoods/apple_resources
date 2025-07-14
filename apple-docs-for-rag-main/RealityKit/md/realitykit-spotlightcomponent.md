

- RealityKit
-  SpotLightComponent 

Structure

# SpotLightComponent

A component that defines a spotlight source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
struct SpotLightComponent
```

## Overview

A spotlight illuminates a cone-shaped volume in the entity’s local forward direction along the z-axis’s negative direction, or `[0.0, 0.0, -1.0]`. Change the a spotlight’s direction with the orientation or look(at:from:upVector:relativeTo:) method, of the Entity with a spotlight component.

The light’s innerAngleInDegrees and outerAngleInDegrees reflect the size of the light’s cone relative to the entity’s forward direction. The light is at full intensity between `0` degrees and innerAngleInDegrees. RealityKit attenuates the light’s intensity between the inner angle and the outer angle. The spotlight’s intensity is `0.0` beyond the outer angle.

Tip

Turn on shadows for a spotlight by adding the SpotLightComponent.Shadow component to an entity that has a `SpotLightComponent`.

The following table shows some real-world scenarios, to better explain how you can use intensity to control the brightness of the light in lumens, and attenuationRadius to control how the level of brightness diminishes with distance from the light source:

| Scenario | Approximate Lumens | Attenuation Radius | Description |
|----|----|----|----|
| Small Accent Spotlight | 100-200 lumens | 5-10 meters | Highlights small objects or artwork |
| LED flashlight | 300-600 lumens | 50-70 meters | Beams a long distance illumination |
| Theatrical Spotlight | 500-1,000 lumens | 20-40 meters | Focuses attention to performers on a stage |
| Outdoor Security Spotlight | 1,000-2,000 lumens | 20-30 meters | Brightly illuminates specific outdoor areas |
| Film/TV Production Spotlight | 5,000-10,000 lumens | 50-100 meters | Provides focused, high-intensity lighting for sets |
| Large-Scale Event Spotlight | 50,000-100,000 lumens | 200-500 meters | Lights large outdoor events or concerts |

## Topics

### Creating a spotlight

init(color: SpotLightComponent.Color, intensity: Float, innerAngleInDegrees: Float, outerAngleInDegrees: Float, attenuationRadius: Float)

Creates a spotlight with the given parameters.

init(color: SpotLightComponent.Color, intensity: Float, innerAngleInDegrees: Float, outerAngleInDegrees: Float, attenuationRadius: Float)

Creates a spotlight with the given parameters.

init(color: SpotLightComponent.Color, intensity: Float, innerAngleInDegrees: Float, outerAngleInDegrees: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a spotlight with the given parameters.

init(color: SpotLightComponent.Color, intensity: Float, innerAngleInDegrees: Float, outerAngleInDegrees: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a spotlight with the given parameters.

### Setting the color

var color: SpotLightComponent.Color

A color for the spotlight.

var color: SpotLightComponent.Color

A color for the spotlight.

### Configuring the spotlight

var intensity: Float

The intensity of the spotlight measured in lumen.

var innerAngleInDegrees: Float

The inner angle of the spotlight in degrees.

var outerAngleInDegrees: Float

The outer angle of the spotlight in degrees.

var attenuationRadius: Float

The distance from the light source where its intensity reaches zero.

var attenuationFalloffExponent: Float

The exponent value for the light’s intensity falloff-transition curve.

### Registering a components type

static func registerComponent()

Registers a new component type.

### Comparing spotlight components

static func == (SpotLightComponent, SpotLightComponent) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Supporting types

typealias Color

A platform-specific type used to define color for a spotlight.

### Structures

struct Shadow

A spotlight component that adds shadows to entities that it illuminates.

### Default Implementations

Component Implementations

Equatable Implementations

## Relationships

### Conforms To

- Component
- Equatable

## See Also

### Spotlights and their shadows

struct Shadow

A spotlight component that adds shadows to entities that it illuminates.

enum ShadowClippingPlane

An object that specifies the mode of a shadow clipping plane.

typealias ShadowMapCullMode

