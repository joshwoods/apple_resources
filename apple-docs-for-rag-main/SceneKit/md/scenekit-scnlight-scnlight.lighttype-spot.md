

- SceneKit
- SCNLight
- SCNLight.LightType
-  spot 

Type Property

# spot

A light source that illuminates a cone-shaped area.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let spot: SCNLight.LightType
```

## Discussion

The position and orientation of the node containing the light determines the area lit by the spotlight, and all lighting attributes affect its appearance.

## See Also

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

static let area: SCNLight.LightType

