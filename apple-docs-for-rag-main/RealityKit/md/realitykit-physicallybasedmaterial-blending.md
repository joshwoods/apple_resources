

- RealityKit
- PhysicallyBasedMaterial
-  blending 

Instance Property

# blending

The transparency of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var blending: PhysicallyBasedMaterial.Blending { get set }
```

## Mentioned in 

Applying realistic material and lighting effects to entities

## Discussion

Use this property to specify whether an entity is opaque or transparent. To create an entity that’s opaque, assign PhysicallyBasedMaterial.Blending.opaque to this property.

```
material.blending = .opaque
```

To create a translucent or transparent object using a single opacity value for the entire material, initialize PhysicallyBasedMaterial.Blending.transparent(opacity:) using a `Float` value.

```
material.blending = .transparent(opacity: .init(floatLiteral:0.5))
```

To use a UV-mapped grayscale image texture to specify different opacity values for different parts of an entity, initialize PhysicallyBasedMaterial.Blending.transparent(opacity:) using a texture. If you provide a color image, RealityKit only uses the intensity of the red channel.

```
if let opacityResource = try? TextureResource.load(named:
"entity_opacity") {
    let opacityMap = MaterialParameterTypes.Texture(opacityResource)
    material.blending = .transparent(opacity: .init(texture: opacityMap))
}
```

## See Also

### Configuring transparency and highlights

var sheen: PhysicallyBasedMaterial.SheenColor?

The intensity of an entity’s sheen.

