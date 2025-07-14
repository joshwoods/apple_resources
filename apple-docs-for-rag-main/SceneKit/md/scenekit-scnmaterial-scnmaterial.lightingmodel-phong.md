

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  phong 

Type Property

# phong

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let phong: SCNMaterial.LightingModel
```

## Discussion

The Phong approximation of real-world reflectance calculates the color of a point on a surface using the following formula:

```
color = ambient * al + diffuse * max(0, dot(N, L)) + specular * pow(max(0, dot(R, E)), shininess)
```

Some terms refer to the material’s properties: ambient, diffuse, specular, and shininess. The other terms are as follows:

`al`  
The sum of all ambient lights in the scene (a color).

`N`  
The surface normal vector at the point being shaded, as supplied by the geometry’s vertex data, interpolated between vertices, and possibly modified by the material’s normal property.

`L`  
The (normalized) vector from the point being shaded to the light source.

`E`  
The (normalized) vector from the point being shaded to the viewer.

`R`  
The reflection of the light vector `L` across the normal vector `N`.

## See Also

### Type Properties

static let blinn: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

static let constant: SCNMaterial.LightingModel

Uniform shading that incorporates ambient lighting only.

static let lambert: SCNMaterial.LightingModel

Shading that incorporates ambient and diffuse properties only.

static let physicallyBased: SCNMaterial.LightingModel

Shading based on a realistic abstraction of physical lights and materials.

static let shadowOnly: SCNMaterial.LightingModel

