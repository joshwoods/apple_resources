

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  constant 

Type Property

# constant

Uniform shading that incorporates ambient lighting only.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let constant: SCNMaterial.LightingModel
```

## Discussion

This shading model calculates the color of a point on a surface with the following formula:

```
color = ambient * al + diffuse
```

The ambient and diffuse terms refer to the material’s properties. The `al` term is the sum of all ambient lights in the scene (a color).

## See Also

### Type Properties

static let blinn: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

static let lambert: SCNMaterial.LightingModel

Shading that incorporates ambient and diffuse properties only.

static let phong: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

static let physicallyBased: SCNMaterial.LightingModel

Shading based on a realistic abstraction of physical lights and materials.

static let shadowOnly: SCNMaterial.LightingModel

