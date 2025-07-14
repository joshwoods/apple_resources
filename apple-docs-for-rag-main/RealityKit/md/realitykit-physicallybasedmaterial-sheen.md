

- RealityKit
- PhysicallyBasedMaterial
-  sheen 

Instance Property

# sheen

The intensity of an entity’s sheen.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var sheen: PhysicallyBasedMaterial.SheenColor? { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

For a PhysicallyBasedMaterial, object, you can use `sheen` to add soft specular highlights that simulate subtle reflections like the ones that occur with some materials, primarily fabrics. You can specify `sheen` using a single color, or you can provide a UV-mapped image.

The following example specifies `sheen` using a single value for the entire material:

```
let sheenColor = PhysicallyBasedMaterial.Color(deviceRed: 0.8,
green: 0.8, blue: 0.8, alpha: 1.0)
material.sheen = .init(tint:sheenColor)
```

This example shows how to specify sheen using a UV-mapped image texture:

```
if let sheenResource = try? TextureResource.load(named:
"entity_sheen") {
    let sheenMap = MaterialParameters.Texture(sheenResource)
    material.sheen = .init(texture: sheenMap)
}
```

## See Also

### Configuring transparency and highlights

var blending: PhysicallyBasedMaterial.Blending

The transparency of an entity.

