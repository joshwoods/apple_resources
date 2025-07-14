

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  lambert 

Type Property

# lambert

Shading that incorporates ambient and diffuse properties only.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let lambert: SCNMaterial.LightingModel
```

## Discussion

This shading model is based on Lambert’s Law of diffuse reflectance, calculating the color of a point on a surface with the following formula:

```
color = ambient * al + diffuse * max(0, dot(N, L))
```

The ambient and diffuse terms refer to the material’s properties. The other terms are as follows:

`al`  
The sum of all ambient lights in the scene (a color).

`N`  
The surface normal vector at the point being shaded, as supplied by the geometry’s vertex data, interpolated between vertices, and possibly modified by the material’s normal property.

`L`  
The (normalized) vector from the point being shaded to the light source.

## See Also

### Type Properties

static let blinn: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

static let constant: SCNMaterial.LightingModel

Uniform shading that incorporates ambient lighting only.

static let phong: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

static let physicallyBased: SCNMaterial.LightingModel

Shading based on a realistic abstraction of physical lights and materials.

static let shadowOnly: SCNMaterial.LightingModel

