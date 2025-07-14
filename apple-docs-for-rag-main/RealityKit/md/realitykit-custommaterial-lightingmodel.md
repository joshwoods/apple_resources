

- RealityKit
- CustomMaterial
-  lightingModel 

Instance Property

# lightingModel

The lighting model that the material uses.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var lightingModel: CustomMaterial.LightingModel { get }
```

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Discussion

A custom material’s lighting model determines exactly how RealityKit uses the values set in your surface shader’s to render the entity.

Custom materials supports the following lighting models:

| Lighting Model | Description | Supported Shader Outputs |
|----|----|----|
| `.lit` | Uses physically based rendering techniques, but excludes clearcoat. | All except `set_clearcoat()` and `set_clearcoat_roughness()` |
| `.clearcoat` | Uses physically based rendering techniques, including clearcoat. | All |
| `.unlit` | Renders without any shading or lighting calculations. The result is similar to using an UnlitMaterial. | Uses `set_emissive_color()` only |

## See Also

### Setting shader properties

var program: CustomMaterial.Program

var custom: CustomMaterial.Custom

User-defined properties for the material’s shader functions.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader and geometry modifier.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, stage: CustomShaderStage, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader or geometry modifier.

