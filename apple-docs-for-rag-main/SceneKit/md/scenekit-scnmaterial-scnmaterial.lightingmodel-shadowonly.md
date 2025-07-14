

- SceneKit
- SCNMaterial
- SCNMaterial.LightingModel
-  shadowOnly 

Type Property

# shadowOnly

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static let shadowOnly: SCNMaterial.LightingModel
```

## See Also

### Type Properties

static let blinn: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Blinn-Phong formula.

static let constant: SCNMaterial.LightingModel

Uniform shading that incorporates ambient lighting only.

static let lambert: SCNMaterial.LightingModel

Shading that incorporates ambient and diffuse properties only.

static let phong: SCNMaterial.LightingModel

Shading that incorporates ambient, diffuse, and specular properties, where specular highlights are calculated using the Phong formula.

static let physicallyBased: SCNMaterial.LightingModel

Shading based on a realistic abstraction of physical lights and materials.

