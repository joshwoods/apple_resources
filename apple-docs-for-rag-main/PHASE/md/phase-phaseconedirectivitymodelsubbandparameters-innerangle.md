

- PHASE
- PHASEConeDirectivityModelSubbandParameters
-  innerAngle 

Instance Property

# innerAngle

An angle, in degrees, that determines the size of the audio emitting area inside the cone.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var innerAngle: Double { get }
```

## Discussion

To set this property, call setAngles(innerAngle:outerAngle:).

## See Also

### Shaping Directivity

var outerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area outside the cone.

var outerGain: Double

The loudness of the audio the outside area of the cone emits.

func setAngles(innerAngle: Double, outerAngle: Double)

Configures a focus area for cone-based sound directivity.

