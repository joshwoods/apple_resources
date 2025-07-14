

- RealityKit
- PhysicallyBasedMaterial
-  normal 

Instance Property

# normal

The normal map for the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var normal: PhysicallyBasedMaterial.Normal { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

*Normal mapping* is a real-time rendering technique that captures fine surface details for a model using a texture instead of increasing the number of polygons in the model. It works by storing *surface normals*, which are vectors perpendicular to the surface of the model, from a much higher resolution version of the same 3D object. A normal map stores each vector in the image by storing the vectors’ `X`, `Y`, and `Z` values as the `R`, `G`, and `B` components of the corresponding pixel in the UV-mapped image.

If you provide a normal map, RealityKit uses the normals stored in the image to do lighting calculations. This results in much more realistic highlights, shadows, and reflections without incurring the computational cost of using a much higher resolution 3D model. RealityKit uses tangent-space normal maps.

The following code loads a normal map texture and uses it to set this property:

```
if let normalResource = try? TextureResource.load(named:
"entity_normals") {
    let normalMap = MaterialParameters.Texture(normalResource)
    material.normal = PhysicallyBasedMaterial.Normal(texture:normalMap)
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

