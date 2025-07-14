

- AVFAudio
-  AVAudioUnitEffect 

Class

# AVAudioUnitEffect

An object that processes audio in real time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitEffect
```

## Overview

This processing uses AudioUnit of type effect, music effect, panner, remote effect, or remote music effect. These effects run in real time and process some number of audio input samples to produce several audio output samples. A delay unit is an example of an effect unit.

## Topics

### Creating an audio effect

init(audioComponentDescription: AudioComponentDescription)

Creates an audio unit effect object with the specified description.

### Getting the bypass state

var bypass: Bool

The bypass state of the audio unit.

## Relationships

### Inherits From

- AVAudioUnit

### Inherited By

- AVAudioUnitDelay
- AVAudioUnitDistortion
- AVAudioUnitEQ
- AVAudioUnitReverb

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio effects

class AVAudioUnitEQ

An object that implements a multiband equalizer.

class AVAudioUnitDistortion

An object that implements a multistage distortion effect.

class AVAudioUnitDelay

An object that implements a delay effect.

class AVAudioUnitReverb

An object that implements a reverb effect.

