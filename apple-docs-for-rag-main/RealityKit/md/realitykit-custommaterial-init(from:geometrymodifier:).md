

- RealityKit
- CustomMaterial
-  init(from:geometryModifier:) 

Initializer

# init(from:geometryModifier:)

Creates a custom material from an existing material and a geometry modifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    from material: any Material,
    geometryModifier: CustomMaterial.GeometryModifier
) throws
```

## Parameters 

`material`  

The material on which to base the custom material.

`geometryModifier`  

The geometry modifier shader function.

## Discussion

Use this initializer to create a custom material with the same properties as another existing material, but with a geometry modifier.

## See Also

### Creating custom materials

init(from: any Material, surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?) throws

Creates a custom material from an existing material, surface shader, and geometry modifier.

init(surfaceShader: CustomMaterial.SurfaceShader, geometryModifier: CustomMaterial.GeometryModifier?, lightingModel: CustomMaterial.LightingModel) throws

Creates a custom material from a lighting model, surface shader, and geometry modifier.

init(program: CustomMaterial.Program)

