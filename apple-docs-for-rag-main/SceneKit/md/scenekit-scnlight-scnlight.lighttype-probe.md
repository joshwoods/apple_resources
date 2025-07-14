

- SceneKit
- SCNLight
- SCNLight.LightType
-  probe 

Type Property

# probe

A sample of the environment around a point in a scene to be used in environment-based lighting.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let probe: SCNLight.LightType
```

## Discussion

A light probe describes a point in a scene in terms of the variations in color and intensity of the illumination it receives from all directions. This information can then be used in shading of materials based on their location in the scene. For example, a white object placed near blue and red walls will appear bluish on surfaces facing the blue wall and reddish on surfaces facing the red wall.

You can place light probes in a scene and generate their lighting contributions using the Xcode scene editor, or import light probes from scene file formats that support them. Lighting-related properties of the SCNLight class do not apply to light probes; their contribution to scene rendering depends entirely on the light probe content generated in Xcode.

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

static let spot: SCNLight.LightType

A light source that illuminates a cone-shaped area.

static let area: SCNLight.LightType

