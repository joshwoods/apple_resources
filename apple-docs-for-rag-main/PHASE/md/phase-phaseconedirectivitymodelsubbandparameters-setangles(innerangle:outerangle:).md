

- PHASE
- PHASEConeDirectivityModelSubbandParameters
-  setAngles(innerAngle:outerAngle:) 

Instance Method

# setAngles(innerAngle:outerAngle:)

Configures a focus area for cone-based sound directivity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
func setAngles(
    innerAngle: Double,
    outerAngle: Double
)
```

## Parameters 

`innerAngle`  

An angle that determines the size of the audio emitting area inside the cone.

`outerAngle`  

An angle that determines the size of the audio emitting area outside the cone.

## Discussion

The default value for each angle is `360.0`. The outer angle needs to be greater than or equal to the inner angle.

## See Also

### Shaping Directivity

var innerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area inside the cone.

var outerAngle: Double

An angle, in degrees, that determines the size of the audio emitting area outside the cone.

var outerGain: Double

The loudness of the audio the outside area of the cone emits.

