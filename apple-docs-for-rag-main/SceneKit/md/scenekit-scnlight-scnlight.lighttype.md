

- SceneKit
- SCNLight
-  SCNLight.LightType 

Structure

# SCNLight.LightType

Constants specifying the general behavior of a light, used by the type property.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct LightType
```

## Overview

Each of the four scenes in the figure below has the same content illuminated by a single SCNLight object. The node containing the light source has the same position and orientation in each scene—all differences between the four pictures are due to the light’s type property.

## Topics

### Type Properties

static let IES: SCNLight.LightType

A light source whose shape, direction, and intensity of illumination is determined by a photometric profile.

static let ambient: SCNLight.LightType

A light that illuminates all objects in the scene from all directions.

static let directional: SCNLight.LightType

A light source with a uniform direction and constant intensity.

static let omni: SCNLight.LightType

An omnidirectional light, also known as a *point light*.

static let probe: SCNLight.LightType

A sample of the environment around a point in a scene to be used in environment-based lighting.

static let spot: SCNLight.LightType

A light source that illuminates a cone-shaped area.

static let area: SCNLight.LightType

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying a Light’s Appearance

var type: SCNLight.LightType

A constant identifying the general behavior of the light.

var color: Any

The color of the light. Animatable.

var temperature: CGFloat

The color temperature, in degrees Kelvin, of the light source. Animatable.

var intensity: CGFloat

The luminous flux, in lumens, or total brightness of the light. Animatable.

var sphericalHarmonicsCoefficients: Data

Data describing the estimated lighting environment in all directions for a light probe.

