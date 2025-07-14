

- AVFAudio
- AVAudioEnvironmentReverbParameters
-  loadFactoryReverbPreset(\_:) 

Instance Method

# loadFactoryReverbPreset(\_:)

Loads one of the reverbs factory presets.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func loadFactoryReverbPreset(_ preset: AVAudioUnitReverbPreset)
```

## Parameters 

`preset`  

A reverb preset to load.

## Discussion

Loading a factory reverb preset changes the sound of the reverb. This is independent of the filter which follows the reverb in the signal chain.

## See Also

### Related Documentation

var enable: Bool

A Boolean value that indicates whether reverberation is in an enabled state.

### Getting and Setting Reverb Values

var level: Float

Controls the amount of reverb, in decibels.

var filterParameters: AVAudioUnitEQFilterParameters

A filter that the system applies to the output.

