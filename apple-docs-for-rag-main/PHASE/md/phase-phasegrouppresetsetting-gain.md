

- PHASE
- PHASEGroupPresetSetting
-  gain 

Instance Property

# gain

The volume of audio playback.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var gain: Double { get }
```

## Discussion

The framework sets the value to the init(gain:rate:gainCurveType:rateCurveType:) parameter, clamped to the range between `0` and `1`. A value of `0` silences the audio and `1` doesn’t modify the audio’s original volume.

## See Also

### Setting Loudness

var gainCurveType: PHASECurveType

A rate of change for the setting’s volume.

