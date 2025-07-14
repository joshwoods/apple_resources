

- SceneKit
- SCNLight
- SCNLight.LightType
-  directional 

Type Property

# directional

A light source with a uniform direction and constant intensity.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let directional: SCNLight.LightType
```

## Discussion

Because a directional light illuminates all objects in the scene from the same direction and with the same intensity, so the position of the node containing the light has no effect. Attenuation and spotlight angle attributes do not apply to directional lights.

## See Also

### Type Properties

static let IES: SCNLight.LightType

A light source whose shape, direction, and intensity of illumination is determined by a photometric profile.

static let ambient: SCNLight.LightType

A light that illuminates all objects in the scene from all directions.

static let omni: SCNLight.LightType

An omnidirectional light, also known as a *point light*.

static let probe: SCNLight.LightType

A sample of the environment around a point in a scene to be used in environment-based lighting.

static let spot: SCNLight.LightType

A light source that illuminates a cone-shaped area.

static let area: SCNLight.LightType

