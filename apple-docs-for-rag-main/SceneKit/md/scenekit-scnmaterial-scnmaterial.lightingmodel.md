

- SceneKit
- SCNMaterial
-  SCNMaterial.LightingModel 

Structure

# SCNMaterial.LightingModel

Constants specifying the lighting and shading algorithm to use for rendering a material.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct LightingModel
```

## Discussion

## Topics

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

static let shadowOnly: SCNMaterial.LightingModel

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Choosing a Shading Model

var lightingModel: SCNMaterial.LightingModel

The lighting formula that SceneKit uses to render the material.

