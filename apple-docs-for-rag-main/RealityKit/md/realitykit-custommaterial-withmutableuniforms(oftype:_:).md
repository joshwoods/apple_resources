

- RealityKit
- CustomMaterial
-  withMutableUniforms(ofType:\_:) 

Instance Method

# withMutableUniforms(ofType:\_:)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader and geometry modifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
mutating func withMutableUniforms(
    ofType: UniformsType.Type,
    _ callback: (inout UniformsType, inout CustomMaterial.ResourceStorage) -> Void
)
```

## Discussion

This method operates like withMutableUniforms(ofType:stage:_:) but sets the same value for all stages at once.

When using this form, ensure that the custom uniforms arguments passed to each stage of your CustomMaterial are of the same type.

## See Also

### Setting shader properties

var program: CustomMaterial.Program

var custom: CustomMaterial.Custom

User-defined properties for the material’s shader functions.

var lightingModel: CustomMaterial.LightingModel

The lighting model that the material uses.

func withMutableUniforms&lt;UniformsType>(ofType: UniformsType.Type, stage: CustomShaderStage, (inout UniformsType, inout CustomMaterial.ResourceStorage&lt;UniformsType>) -> Void)

Calls the given closure with an inout reference to the underlying storage bound to the custom uniforms argument of a surface shader or geometry modifier.

