

- RealityKit
- PhysicallyBasedMaterial
-  specular 

Instance Property

# specular

The specular highlight applied to the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var specular: PhysicallyBasedMaterial.Specular { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

In Physically Based Rendering (PBR), specular highlights primarily come from the object’s roughness value. RealityKit automatically renders materials that have a low roughness value with specular highlights based on the environment lighting and the shape of the entity. As a result, for most materials, you won’t need to specify a `specular` value when using PhysicallyBasedMaterial.

For some types of dielectric (nonmetallic) materials, like facet-cut glass or gems, PBR algorithms don’t create bright enough specular highlights using just roughness. To accurately simulate those types of materials, use the specular property to specify additional specular for the entity.

The following example demonstrates how to specify specular using a single value for the entire material:

```
material.specular = .init(floatLiteral: 0.8)
```

This example shows how to specify specular using a UV-mapped image texture:

```
if let specularResource = try? TextureResource.load(named:"entity_specular") {
    let specularMap = MaterialParameters.Texture(specularResource)
    material.specular = .init(texture: specularMap)
}
```

## See Also

### Setting the core properties

var baseColor: PhysicallyBasedMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: PhysicallyBasedMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

var metallic: PhysicallyBasedMaterial.Metallic

The reflectiveness of an entity.

var normal: PhysicallyBasedMaterial.Normal

The normal map for the entity.

var ambientOcclusion: PhysicallyBasedMaterial.AmbientOcclusion

The ambient occlusion values for a material.

var clearcoat: PhysicallyBasedMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: PhysicallyBasedMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: PhysicallyBasedMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

