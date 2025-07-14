

- RealityKit
- PhysicallyBasedMaterial
-  emissiveIntensity 

Instance Property

# emissiveIntensity

The intensity of light emitted by the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var emissiveIntensity: Float { get set }
```

## Discussion

To make a material *emissive* and appear to emit light, set this property to a value greater than zero and set emissiveColor to a value other than black. RealityKit multiplies emissiveColor by this value, so the higher the value, the more intense the entity’s emission of light.

You can set this property to values greater than `1.0`.

## See Also

### Adding light emission

var emissiveColor: PhysicallyBasedMaterial.EmissiveColor

The color of the light the entity emits.

