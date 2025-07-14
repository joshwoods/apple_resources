

- PHASE
- PHASEGroup
-  gain 

Instance Property

# gain

Modifies the volume of the group’s sounds.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gain: Double { get set }
```

## Discussion

This property modifies the volume of all audio in the group. The framework clamps the value to the range between `0` and `1`, where `0` silences the audio and `1` doesn’t modify the original volume.

## See Also

### Conrolling Loudness

func fadeGain(gain: Double, duration: Double, curveType: PHASECurveType)

Adjusts the volume of the sounds in a group gradually.

