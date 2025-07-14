

- RealityKit
- PhysicallyBasedMaterial
-  roughness 

Instance Property

# roughness

The amount the surface of the 3D object scatters reflected light.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var roughness: PhysicallyBasedMaterial.Roughness { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

The `roughness` property represents how much the surface of the entity scatters light it reflects. A material with a high roughness has a matte appearance, while one with a low roughness has a shiny appearance.

Specify this property using a Float to represent a uniform `roughness` for the entire entity, or a UV-mapped grayscale image that uses shades of gray to represent the roughness of different parts of the entity. When using an image, black pixels represent areas that have a low roughness and appear shiny, while white represents areas that have a high roughness and display a matte finish.

If you initialize this property with a color image rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

The following example uses a single value to specify roughness:

```
material.roughness = PhysicallyBasedMaterial.Roughness(floatLiteral: 0.0)
```

The following example uses an image to specify roughness:

```
if let roughnessResource = try? TextureResource.load(named:
"entity_roughness") {
    let roughness = MaterialParameters.Texture(roughnessResource)
    material.roughness = PhysicallyBasedMaterial.Roughness(texture:roughness)
}
```

## See Also

### Setting the core properties

var baseColor: PhysicallyBasedMaterial.BaseColor

The color of an entity unmodified by lighting.

var metallic: PhysicallyBasedMaterial.Metallic

The reflectiveness of an entity.

var normal: PhysicallyBasedMaterial.Normal

The normal map for the entity.

var ambientOcclusion: PhysicallyBasedMaterial.AmbientOcclusion

The ambient occlusion values for a material.

var specular: PhysicallyBasedMaterial.Specular

The specular highlight applied to the entity.

var clearcoat: PhysicallyBasedMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: PhysicallyBasedMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: PhysicallyBasedMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

