

- SceneKit
- SCNLight
- SCNLight.LightType
-  omni 

Type Property

# omni

An omnidirectional light, also known as a *point light*.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let omni: SCNLight.LightType
```

## Discussion

Because an omnidirectional light casts equal illumination in all directions, the orientation of the node containing the light has no effect. Spotlight angle and shadow attributes do not apply to directional lights.

## See Also

### Type Properties

static let IES: SCNLight.LightType

A light source whose shape, direction, and intensity of illumination is determined by a photometric profile.

static let ambient: SCNLight.LightType

A light that illuminates all objects in the scene from all directions.

static let directional: SCNLight.LightType

A light source with a uniform direction and constant intensity.

static let probe: SCNLight.LightType

A sample of the environment around a point in a scene to be used in environment-based lighting.

static let spot: SCNLight.LightType

A light source that illuminates a cone-shaped area.

static let area: SCNLight.LightType

