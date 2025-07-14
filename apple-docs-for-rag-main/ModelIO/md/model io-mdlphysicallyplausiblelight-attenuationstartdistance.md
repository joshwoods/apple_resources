

- Model I/O
- MDLPhysicallyPlausibleLight
-  attenuationStartDistance 

Instance Property

# attenuationStartDistance

The distance from the light source, in units of local coordinate space, at which its illumination begins to diminish.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var attenuationStartDistance: Float { get set }
```

## Discussion

At distances less than the start distance, the light’s illumination is at full intensity. At distances greater than the end distance, the light provides no illumination. At distances in between the start and end distance, the attenuationFalloffExponent property defines the transition from full illumination to no illumination.

The default distance is `1.0`.

## See Also

### Managing Attenuation

var attenuationEndDistance: Float

The distance from the light source, in units of local coordinate space, at which its illumination becomes zero.

