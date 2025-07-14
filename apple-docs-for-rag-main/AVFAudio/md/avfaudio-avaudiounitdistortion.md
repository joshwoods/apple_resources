

- AVFAudio
-  AVAudioUnitDistortion 

Class

# AVAudioUnitDistortion

An object that implements a multistage distortion effect.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitDistortion
```

## Topics

### Configuring the distortion

func loadFactoryPreset(AVAudioUnitDistortionPreset)

Configures the audio distortion unit by loading a distortion preset.

enum AVAudioUnitDistortionPreset

Constants that represent preset audio distortions.

### Getting and setting the distortion values

var preGain: Float

The gain that the audio unit applies to the signal before distortion, in decibels.

var wetDryMix: Float

The blend of the distorted and dry signals.

## Relationships

### Inherits From

- AVAudioUnitEffect

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio effects

class AVAudioUnitEffect

An object that processes audio in real time.

class AVAudioUnitEQ

An object that implements a multiband equalizer.

class AVAudioUnitDelay

An object that implements a delay effect.

class AVAudioUnitReverb

An object that implements a reverb effect.

