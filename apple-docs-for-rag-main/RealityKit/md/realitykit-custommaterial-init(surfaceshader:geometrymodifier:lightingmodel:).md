

- RealityKit
- CustomMaterial
-  init(surfaceShader:geometryModifier:lightingModel:) 

Initializer

# init(surfaceShader:geometryModifier:lightingModel:)

Creates a custom material from a lighting model, surface shader, and geometry modifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    surfaceShader: CustomMaterial.SurfaceShader,
    geometryModifier: CustomMaterial.GeometryModifier? = nil,
    lightingModel: CustomMaterial.LightingModel
) throws
```

## Parameters 

`surfaceShader`  

The surface shader function.

`geometryModifier`  

The geometry modifier shader function.

`lightingModel`  

The lighting model.

## Mentioned in 

Modifying RealityKit rendering using custom materials

## Discussion

This initializer creates a custom material using a lighting model you specify, which determines how RealityKit renders the output of your shader functions. The CustomMaterial.LightingModel.lit and CustomMaterial.LightingModel.clearcoat use RealityKit’s physically-based shaders to render the entity based on the output of your shader functions. When using these lighting models, RealityKit uses all provided material attributes like baseColor, metallic and normal.

The CustomMaterial.LightingModel.unlit lighting model renders the entity with no shadows or surface effects. This lighting model only supports baseColor and blending.

## See Also

### Creating custom materials

init(from: any Material, geometryModifier: CustomMaterial.GeometryModifier) throws

Creates a custom material from an existing material and a geometry modifier.

init(from: any Material, surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?) throws

Creates a custom material from an existing material, surface shader, and geometry modifier.

init(program: CustomMaterial.Program)

