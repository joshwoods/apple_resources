

- RealityKit
- PhysicallyBasedMaterial
-  ambientOcclusion 

Instance Property

# ambientOcclusion

The ambient occlusion values for a material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var ambientOcclusion: PhysicallyBasedMaterial.AmbientOcclusion { get set }
```

## Discussion

Ambient occlusion represents the entity’s exposure to ambient light.

Specify ambient occlusion using a UV-mapped image called an *ambient occlusion map*. A value of black (`0.0`) represents parts of the model that receive less ambient light because that part of the model is a crevice, dent, or recessed area, or because another part of the same entity is preventing ambient light from reaching it. Ambient occlusion values of white (`1.0`) represent flat portions of the model that receive full ambient light. You generate ambient occlusion maps using a 3D software package.

The following code loads an ambient occlusion map:

```
"entity_ao") {
    let aoMap = MaterialParameters.Texture(aoResource)
    material.emissiveColor = .init(texture: aoMap)
} ```
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

var specular: PhysicallyBasedMaterial.Specular

The specular highlight applied to the entity.

var clearcoat: PhysicallyBasedMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: PhysicallyBasedMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: PhysicallyBasedMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

