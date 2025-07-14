

- AVFoundation
-  AVAudioMixInputParameters 

Class

# AVAudioMixInputParameters

An object that represents the parameters that you apply when adding an audio track to a mix.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVAudioMixInputParameters
```

## Overview

You use an instance `AVAudioMixInputParameters` to apply audio volume ramps for an input to an audio mix. Mix parameters are associated with audio tracks via the trackID property.

Audio volume is currently supported as a time-varying parameter. `AVAudioMixInputParameters` has a mutable subclass, AVMutableAudioMixInputParameters.

Before the first time at which a volume is set, a volume of 1.0 used; after the last time for which a volume has been set, the last volume is used. Within the time range of a volume ramp, the volume is interpolated between the start volume and end volume of the ramp. For example, setting the volume to 1.0 at time 0 and also setting a volume ramp from a volume of 0.5 to 0.2 with a timeRange of \[4.0, 5.0\] results in an audio volume parameters that hold the volume constant at 1.0 from 0.0 sec to 4.0 sec, then cause it to jump to 0.5 and descend to 0.2 from 4.0 sec to 9.0 sec, holding constant at 0.2 thereafter.

Given that this is an immutable variant of the object, you should not allocate and initialize a version of this class yourself. Other classes may return instances of this class.

## Topics

### Getting the Track ID

var trackID: CMPersistentTrackID

The identifier of the audio track to which the parameters should be applied.

### Getting Volume Ramps

func getVolumeRamp(for: CMTime, startVolume: UnsafeMutablePointer&lt;Float>?, endVolume: UnsafeMutablePointer&lt;Float>?, timeRange: UnsafeMutablePointer&lt;CMTimeRange>?) -> Bool

Retrieves the volume ramp that includes the specified time.

### Getting an Audio Tap

var audioTapProcessor: MTAudioProcessingTap?

The audio processing tap associated with the track.

### Getting the Time Pitch Algorithm Setting

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm?

The processing algorithm used to manage audio pitch for scaled audio edits.

struct AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableAudioMixInputParameters

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Mixing

class AVAudioMix

An object that manages the input parameters for mixing audio tracks.

class AVMutableAudioMix

An object that manages the input parameters for mixing audio tracks.

class AVMutableAudioMixInputParameters

The parameters you use when adding an audio track to a mix.

