

- RealityKit
- PhysicallyBasedMaterial
-  clearcoat 

Instance Property

# clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var clearcoat: PhysicallyBasedMaterial.Clearcoat { get set }
```

## Discussion

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear transparent coating, like the paint on a car, or the surface of lacquered objects. By default, materials don’t have clearcoat enabled.

Use this property to enable clearcoat rendering. Specifying any value greater than `0.0` turns clearcoat rendering on. A value of `1.0` indicates a full clearcoat. RealityKit treats values above `1.0` as if they’re `1.0`.

You can specify clearcoat using a single `Float` that applies to the entire material, or a UV-mapped grayscale image to provide different values for different parts of an entity.

The following example specifies `clearcoat` using a single value:

```
material.clearcoat = .init(floatLiteral: 0.8)
```

And this example shows how to specify `clearcoat` using a UV-mapped image texture:

```
if let clearcoatResource = try? TextureResource.load(named:"entity_clearcoat") {
    let clearcoatMap = MaterialParameters.Texture(clearcoatResource)
    material.clearcoat = .init(texture: clearcoatMap)
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

var specular: PhysicallyBasedMaterial.Specular

The specular highlight applied to the entity.

var clearcoatRoughness: PhysicallyBasedMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: PhysicallyBasedMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

