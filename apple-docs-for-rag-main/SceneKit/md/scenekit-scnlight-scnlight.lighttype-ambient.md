

- SceneKit
- SCNLight
- SCNLight.LightType
-  ambient 

Type Property

# ambient

A light that illuminates all objects in the scene from all directions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let ambient: SCNLight.LightType
```

## Discussion

Because the intensity of light from an ambient source is the same everywhere in the scene, its position and direction have no effect. Attenuation, spotlight angle, and shadow attributes do not apply to ambient lights.

## See Also

### Type Properties

static let IES: SCNLight.LightType

A light source whose shape, direction, and intensity of illumination is determined by a photometric profile.

static let directional: SCNLight.LightType

A light source with a uniform direction and constant intensity.

static let omni: SCNLight.LightType

An omnidirectional light, also known as a *point light*.

static let probe: SCNLight.LightType

A sample of the environment around a point in a scene to be used in environment-based lighting.

static let spot: SCNLight.LightType

A light source that illuminates a cone-shaped area.

static let area: SCNLight.LightType

