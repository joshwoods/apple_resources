

- RealityKit
- PhysicallyBasedMaterial
-  anisotropyLevel 

Instance Property

# anisotropyLevel

The degree to which an entity reflects light to create stretched or oblong highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var anisotropyLevel: PhysicallyBasedMaterial.AnisotropyLevel { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

By default, PBR materials are isotropic; in other words, an entity that uses PhysicallyBasedMaterial reflects light uniformly in all directions, mimicking the behavior of most real-world objects. Some objects, including those with many small parallel striations such as vinyl records, CDs, or straight hair, reflect light more in some directions than others, resulting in stretched or oblong specular highlights, as shown in the following figure.

This property controls the amount of anisotropy. It works together with anisotropyAngle, which defines the angle of elongation for the specular highlights.

The following example specifies `anisotropyLevel` using single values for the entire material:

```
material.anisotropyLevel = .AnisotropyLevel(floatLiteral: 0.5)
```

This example specifies `anisotropyLevel` using a UV-mapped image texture.

```
if let anisoLevelResource = try? TextureResource.load(named:
"entity_aniso_level") {
    let anisoLevelMap = MaterialParameters.Texture(sheenResource)
    material.anisotropyLevel = .init(texture: anisoLevelMap)
}
```

## See Also

### Adding anisotropy

var anisotropyAngle: PhysicallyBasedMaterial.AnisotropyAngle

The angle at which the anisotropic direction of the material is oriented, influencing the reflection and appearance of surface highlights.

