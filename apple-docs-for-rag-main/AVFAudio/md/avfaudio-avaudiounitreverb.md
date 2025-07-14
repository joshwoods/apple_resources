

- AVFAudio
-  AVAudioUnitReverb 

Class

# AVAudioUnitReverb

An object that implements a reverb effect.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitReverb
```

## Overview

A reverb simulates the acoustic characteristics of a particular environment. Use the different presets to simulate a particular space and blend it in with the original signal using the wetDryMix property.

## Topics

### Configure the reverb

func loadFactoryPreset(AVAudioUnitReverbPreset)

Configures the audio unit as a reverb preset.

enum AVAudioUnitReverbPreset

Constants that represent preset reverbs.

### Getting and setting the reverb values

var wetDryMix: Float

The blend of the wet and dry signals.

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

class AVAudioUnitDistortion

An object that implements a multistage distortion effect.

class AVAudioUnitDelay

An object that implements a delay effect.

