

- AVFAudio
- AVAudioPlayer
-  volume 

Instance Property

# volume

The audio player’s volume relative to other audio output.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var volume: Float { get set }
```

## Discussion

This property supports values ranging from `0.0` for silence to `1.0` for full volume.

## See Also

### Configuring playback settings

func setVolume(Float, fadeDuration: TimeInterval)

Changes the audio player’s volume over a duration of time.

var pan: Float

The audio player’s stereo pan position.

var enableRate: Bool

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var rate: Float

The audio player’s playback rate.

var numberOfLoops: Int

The number of times the audio repeats playback.

