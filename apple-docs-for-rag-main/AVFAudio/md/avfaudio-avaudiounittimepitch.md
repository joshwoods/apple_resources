

- AVFAudio
-  AVAudioUnitTimePitch 

Class

# AVAudioUnitTimePitch

An object that provides a good-quality playback rate and pitch shifting independently of each other.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAudioUnitTimePitch
```

## Topics

### Getting and setting time pitch values

var overlap: Float

The amount of overlap between segments of the input audio signal.

var pitch: Float

The amount to use to pitch shift the input signal.

var rate: Float

The playback rate of the input signal.

## Relationships

### Inherits From

- AVAudioUnitTimeEffect

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Time effects

class AVAudioUnitTimeEffect

An object that processes audio in nonreal time.

class AVAudioUnitVarispeed

An object that allows control of the playback rate.

