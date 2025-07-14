

- AVFoundation
-  AVMutableAudioMixInputParameters 

Class

# AVMutableAudioMixInputParameters

The parameters you use when adding an audio track to a mix.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVMutableAudioMixInputParameters
```

## Topics

### Creating Input Parameters

convenience init(track: AVAssetTrack?)

Creates a mutable input parameters object for a given track.

### Managing the Track ID

var trackID: CMPersistentTrackID

The identifier of the audio track to which the parameters should be applied.

### Setting the Volume

func setVolume(Float, at: CMTime)

Sets the value of the audio volume starting at the specified time.

func setVolumeRamp(fromStartVolume: Float, toEndVolume: Float, timeRange: CMTimeRange)

Sets a volume ramp to apply during a specified time range.

### Getting an Audio Tap

var audioTapProcessor: MTAudioProcessingTap?

The audio processing tap associated with the track.

### Time Pitch Settings

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm?

The processing algorithm used to manage audio pitch for scaled audio edits.

struct AVAudioTimePitchAlgorithm

An algorithm used to set the audio pitch as the rate changes.

## Relationships

### Inherits From

- AVAudioMixInputParameters

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

class AVAudioMixInputParameters

An object that represents the parameters that you apply when adding an audio track to a mix.

