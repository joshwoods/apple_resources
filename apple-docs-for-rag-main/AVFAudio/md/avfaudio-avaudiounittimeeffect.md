

- AVFAudio
-  AVAudioUnitTimeEffect 

Class

# AVAudioUnitTimeEffect

An object that processes audio in nonreal time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitTimeEffect
```

## Overview

A time effect audio unit represents an AVAudioUnit with a type `kAudioUnitType_FormatConverter` (`aufc)`. These effects don’t process audio in real time. The AVAudioUnitVarispeed class is an example of a time effect unit.

## Topics

### Creating a time effect

init(audioComponentDescription: AudioComponentDescription)

Creates a time effect audio unit with the specified description.

### Getting and setting the time effect

var bypass: Bool

The bypass state of the audio unit.

## Relationships

### Inherits From

- AVAudioUnit

### Inherited By

- AVAudioUnitTimePitch
- AVAudioUnitVarispeed

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Time effects

class AVAudioUnitTimePitch

An object that provides a good-quality playback rate and pitch shifting independently of each other.

class AVAudioUnitVarispeed

An object that allows control of the playback rate.

