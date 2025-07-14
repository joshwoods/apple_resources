

- AVFAudio
- AVAudioUnitDistortion
-  loadFactoryPreset(\_:) 

Instance Method

# loadFactoryPreset(\_:)

Configures the audio distortion unit by loading a distortion preset.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func loadFactoryPreset(_ preset: AVAudioUnitDistortionPreset)
```

## Parameters 

`preset`  

The distortion preset.

## Discussion

For more information about possible values for `preset`, see AVAudioUnitDistortionPreset. The default value is AVAudioUnitDistortionPreset.drumsBitBrush.

## See Also

### Configuring the distortion

enum AVAudioUnitDistortionPreset

Constants that represent preset audio distortions.

