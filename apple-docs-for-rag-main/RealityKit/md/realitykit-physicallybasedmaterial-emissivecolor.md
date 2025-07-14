

- RealityKit
- PhysicallyBasedMaterial
-  emissiveColor 

Instance Property

# emissiveColor

The color of the light the entity emits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var emissiveColor: PhysicallyBasedMaterial.EmissiveColor { get set }
```

## Discussion

With Physically Based Rendering (PBR), you can give entities in RealityKit the appearance of emitting light. Use this property to simulate real-world objects that glow, such as objects with LEDs or computer screens. To enable light emission from a material, set emissiveIntensity to a value greater than zero, then specify a color for the emitted light other than black using this property. You can specify a single emissive color for the entire material, or use a UV-mapped image texture to use different colors for different parts of the entity.

The following example uses a single color for the entire material:

```
material.emissiveIntensity = 2.0
self.emissiveColor = PhysicallyBasedMaterial.EmissiveColor(color: .red)
```

This example uses an image map to control the light emission color:

```
if let emissiveResource = try? TextureResource.load(named:"entity_emissive") {
    let emissiveMap = MaterialParameters.Texture(emissiveResource)
    material.emissiveColor = .init(texture: emissiveMap)
}
```

## See Also

### Adding light emission

var emissiveIntensity: Float

The intensity of light emitted by the entity.

