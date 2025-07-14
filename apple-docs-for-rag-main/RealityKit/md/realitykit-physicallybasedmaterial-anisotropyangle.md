

- RealityKit
- PhysicallyBasedMaterial
-  anisotropyAngle 

Instance Property

# anisotropyAngle

The angle at which the anisotropic direction of the material is oriented, influencing the reflection and appearance of surface highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var anisotropyAngle: PhysicallyBasedMaterial.AnisotropyAngle { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

This property controls the scattering angle for anisotropic objects. If anisotropyLevel is `0.0`, this property has no effect. This property takes a value between `0.0 `and `1.0` or a UV-mapped grayscale image specifying angles for different parts of the entity.` A` value of black (`0.0)` means a rotation of 0° and a value of white (`1.0)` indicates a rotation of 360°. To determine the anisotropyAngle value from an angle, divide the desired angle in degrees by `360.0` or the desired angle in radians by pi times 2.

```
let angleDegrees = Float(125.0)
let anisotropyAngleFromDegrees = angleDegrees / 360.0

let angleRadians = Float(2.181662) let anisotropyAngleFromRadians =
angleRadians / (Float.pi * Float(2.0))
```

The following example shows how to specify `anisotropyAngle` using single values for the entire material:

```
material.anisotropyAngle = .AnisotropyAngle(floatLiteral: 0.25)
```

This example shows how to specify anisotropy using a UV-mapped image texture for anisotropyLevel and a separate image for anisotropyAngle:

```
if let anisoLevelResource = try? TextureResource.load(named:
"entity_aniso_level") {
    let anisoLevelMap = MaterialParameters.Texture(sheenResource)
    material.anisotropyLevel = .init(texture: anisoLevelMap)
}
if let anisoAngleResource = try? TextureResource.load(named:
"entity_aniso_angle") {
    let anisoAngleMap = MaterialParameters.Texture(anisoAngleResource)
    material.anisotropyAngle = .init(texture: anisoAngleMap)
}
```

## See Also

### Adding anisotropy

var anisotropyLevel: PhysicallyBasedMaterial.AnisotropyLevel

The degree to which an entity reflects light to create stretched or oblong highlights.

