

- RealityKit
- PhysicallyBasedMaterial
-  metallic 

Instance Property

# metallic

The reflectiveness of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var metallic: PhysicallyBasedMaterial.Metallic { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

The `metallic` property represents the reflectiveness of an entity. Use this property to specify whether the entity displays metallic qualities and reflects the surrounding environment, or displays dielectric qualities and doesn’t reflect the environment.

Specify this property using a Float to represent a uniform reflectiveness for the entire entity. You an also use a UV-mapped grayscale image to represent the reflectiveness of different parts of the entity. When using an image, black pixels represent areas that are dielectric, while white pixels represents areas that are completely metallic and reflective.

If you initialize this property with a color image, rather than a grayscale image, RealityKit only uses the intensity of the image’s red channel.

The following example specifies the metallic qualities of an entity using a single float value:

```
material.metallic = 1.0
```

The following example specifies the metallic qualities of an entity using a UV-mapped image:

```
// Load a texture resource from a file.
let metalResource = try TextureResource.load(named: "entity_metallic")

// Set the texture to the metallic property.
let metallic = MaterialParameters.Texture(metalResource)
material.metallic = PhysicallyBasedMaterial.Metallic(texture: metallic)
```

## See Also

### Setting the core properties

var baseColor: PhysicallyBasedMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: PhysicallyBasedMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

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

