

- SceneKit
- SCNLight
- SCNLight.LightType
-  IES 

Type Property

# IES

A light source whose shape, direction, and intensity of illumination is determined by a photometric profile.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let IES: SCNLight.LightType
```

## Discussion

The intensity of a photometric light varies in different directions from the light source, much like the illumination from a real-world light source. The position of the containing node determines the location of the light source, and the orientation of the node determines the relative directions specified by the photometric profile. Spotlight angle attributes do not apply to photometric lights.

For more information about photometric lights, see the iesProfileURL property.

## See Also

### Type Properties

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

