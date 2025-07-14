

- AVFAudio
-  AVAudioUnitDelay 

Class

# AVAudioUnitDelay

An object that implements a delay effect.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitDelay
```

## Overview

A delay unit delays the input signal by the specified time interval and then blends it with the input signal. You can also control the amount of high-frequency roll-off to simulate the effect of a tape delay.

## Topics

### Getting and setting the delay values

var delayTime: TimeInterval

The time for the input signal to reach the output.

var feedback: Float

The amount of the output signal that feeds back into the delay line.

var lowPassCutoff: Float

The cutoff frequency above which high frequency content rolls off, in hertz.

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

class AVAudioUnitReverb

An object that implements a reverb effect.

