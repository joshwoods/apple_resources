

- AVFAudio
- AVAudioPlayer
-  pan 

Instance Property

# pan

The audio player’s stereo pan position.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var pan: Float { get set }
```

## Discussion

Set this property value to position the audio in the stereo field. Use a value of `-1.0` to indicate full left, `1.0` for full right, and `0.0` for center.

## See Also

### Configuring playback settings

var volume: Float

The audio player’s volume relative to other audio output.

func setVolume(Float, fadeDuration: TimeInterval)

Changes the audio player’s volume over a duration of time.

var enableRate: Bool

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var rate: Float

The audio player’s playback rate.

var numberOfLoops: Int

The number of times the audio repeats playback.

