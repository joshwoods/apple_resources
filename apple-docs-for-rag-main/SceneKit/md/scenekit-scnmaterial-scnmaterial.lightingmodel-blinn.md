

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  blinn 

Type Property

# blinn

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let blinn: SCNMaterial.LightingModel
```

## Discussion

The Blinn-Phong approximation of real-world reflectance calculates the color of a point on a surface using the following formula:

```
color = ambient * al + diffuse * max(0, dot(N, L)) + specular * pow(max(0, dot(H, N)), shininess)
```

Some terms refer to the material’s properties: ambient, diffuse, specular, and shininess. The other terms are as follows:

`al`  
The sum of all ambient lights in the scene (a color).

`N`  
The surface normal vector at the point being shaded, as supplied by the geometry’s vertex data, interpolated between vertices, and possibly modified by the material’s normal property.

`L`  
The (normalized) vector from the point being shaded to the light source.

`H`  
A vector halfway between the light vector `L` and the (normalized) eye vector `E` (the vector from the point being shaded to the viewer), calculated using the formula `H = normalize(L + E)`.

## See Also

### Type Properties

static let constant: SCNMaterial.LightingModel

Uniform shading that incorporates ambient lighting only.

static let lambert: SCNMaterial.LightingModel

Shading that incorporates ambient and diffuse properties only.

static let phong: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

static let physicallyBased: SCNMaterial.LightingModel

Shading based on a realistic abstraction of physical lights and materials.

static let shadowOnly: SCNMaterial.LightingModel

