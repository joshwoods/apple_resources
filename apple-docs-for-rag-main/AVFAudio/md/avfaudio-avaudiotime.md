

- AVFAudio
-  AVAudioTime 

Class

# AVAudioTime

An object you use to represent a moment in time.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class AVAudioTime
```

## Overview

The `AVAudioTime` object represents a single moment in time in two ways:

- As host time, using the system’s basic clock with `mach_absolute_time()`

- As audio samples at a particular sample rate

A single `AVAudioTime` instance contains either or both representations, meaning it might represent only a sample time, a host time, or both.

Instances of this class are immutable.

## Topics

### Creating an Audio Time Instance

init(audioTimeStamp: UnsafePointer&lt;AudioTimeStamp>, sampleRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

init(hostTime: UInt64)

Creates an audio time object with the specified host time.

init(hostTime: UInt64, sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified host time, sample time, and sample rate.

init(sampleTime: AVAudioFramePosition, atRate: Double)

Creates an audio time object with the specified timestamp and sample rate.

func extrapolateTime(fromAnchor: AVAudioTime) -> AVAudioTime?

Creates an audio time object by converting between host time and sample time.

### Manipulating Host Time

var hostTime: UInt64

The host time.

var isHostTimeValid: Bool

A Boolean value that indicates whether the host time value is valid.

class func hostTime(forSeconds: TimeInterval) -> UInt64

Converts seconds to host time.

class func seconds(forHostTime: UInt64) -> TimeInterval

Converts host time to seconds.

### Getting Sample Rate Information

var sampleRate: Double

The sampling rate that the sample time property expresses.

var sampleTime: AVAudioFramePosition

The time as a number of audio samples that the current audio device tracks.

var isSampleTimeValid: Bool

A Boolean value that indicates whether the sample time and sample rate properties are in a valid state.

### Getting the Core Audio Time Stamp

var audioTimeStamp: AudioTimeStamp

The time as an audio timestamp.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Supporting data types

class AVAudioBuffer

An object that represents a buffer of audio data with a format.

class AVAudioFile

An object that represents an audio file that the system can open for reading or writing.

Audio settings

Configure audio processing settings using standard key and value constants.

