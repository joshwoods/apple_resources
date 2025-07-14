

- AVFAudio
- AVAudioUnitReverb
-  loadFactoryPreset(\_:) 

Instance Method

# loadFactoryPreset(\_:)

Configures the audio unit as a reverb preset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func loadFactoryPreset(_ preset: AVAudioUnitReverbPreset)
```

## Parameters 

`preset`  

The reverb preset.

## Discussion

For more information about possible values, see AVAudioUnitReverbPreset. The default value is AVAudioUnitReverbPreset.mediumHall.

## See Also

### Configure the reverb

enum AVAudioUnitReverbPreset

Constants that represent preset reverbs.

