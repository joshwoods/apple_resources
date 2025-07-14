

- AVFAudio
- AVAudioPlayer
-  setVolume(\_:fadeDuration:) 

Instance Method

# setVolume(\_:fadeDuration:)

Changes the audio player’s volume over a duration of time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func setVolume(
    _ volume: Float,
    fadeDuration duration: TimeInterval
)
```

## Parameters 

`volume`  

The target volume.

`duration`  

The duration, in seconds, over which to fade the volume.

## See Also

### Configuring playback settings

var volume: Float

The audio player’s volume relative to other audio output.

var pan: Float

The audio player’s stereo pan position.

var enableRate: Bool

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var rate: Float

The audio player’s playback rate.

var numberOfLoops: Int

The number of times the audio repeats playback.

