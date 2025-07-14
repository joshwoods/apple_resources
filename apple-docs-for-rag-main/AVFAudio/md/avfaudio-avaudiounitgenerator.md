

- AVFAudio
-  AVAudioUnitGenerator 

Class

# AVAudioUnitGenerator

An object that generates audio output.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitGenerator
```

## Overview

A generator represents an AudioUnit of type `kAudioUnitType_Generator` or `kAudioUnitType_RemoteGenerator`. A generator has no audio input, but produces audio output. An example is a tone generator.

## Topics

### Creating an audio unit generator

init(audioComponentDescription: AudioComponentDescription)

Creates a generator audio unit with the specified description.

### Getting and setting the bypass status

var bypass: Bool

The bypass state of the audio unit.

## Relationships

### Inherits From

- AVAudioUnit

### Conforms To

- AVAudio3DMixing
- AVAudioMixing
- AVAudioStereoMixing
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

