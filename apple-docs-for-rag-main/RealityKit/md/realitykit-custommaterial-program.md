

- RealityKit
- CustomMaterial
-  program 

Instance Property

# program

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var program: CustomMaterial.Program { get set }
```

## See Also

### Setting shader properties

var custom: CustomMaterial.Custom

User-defined properties for the material’s shader functions.

var lightingModel: CustomMaterial.LightingModel

The lighting model that the material uses.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader and geometry modifier.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, stage: CustomShaderStage, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader or geometry modifier.

