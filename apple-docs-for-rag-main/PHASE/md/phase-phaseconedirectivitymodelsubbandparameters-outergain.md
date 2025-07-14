

- PHASE
- PHASEConeDirectivityModelSubbandParameters
-  outerGain 

Instance Property

# outerGain

The loudness of the audio the outside area of the cone emits.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var outerGain: Double { get set }
```

## Discussion

The framework clamps the value of this property to the range `[0,` `1]`, where `0` silences loudness and `1` doesn’t modify loudness.

## See Also

### Shaping Directivity

var innerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area inside the cone.

var outerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area outside the cone.

func setAngles(innerAngle: Double, outerAngle: Double)

Configures a focus area for cone-based sound directivity.

