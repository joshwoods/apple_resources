

- AVFAudio
-  AVAudioUnitEQ 

Class

# AVAudioUnitEQ

An object that implements a multiband equalizer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitEQ
```

## Overview

The AVAudioUnitEQFilterParameters class encapsulates the filter parameters that the bands property array returns.

## Topics

### Creating an equalizer

init(numberOfBands: Int)

Creates an audio unit equalizer object with the specified number of bands.

### Getting and setting the equalizer values

class AVAudioUnitEQFilterParameters

An object that encapsulates the parameters that the equalizer uses.

var bands: [AVAudioUnitEQFilterParameters]

An array of equalizer filter parameters.

var globalGain: Float

The overall gain adjustment that the audio unit applies to the signal, in decibels.

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

class AVAudioUnitDistortion

An object that implements a multistage distortion effect.

class AVAudioUnitDelay

An object that implements a delay effect.

class AVAudioUnitReverb

An object that implements a reverb effect.

