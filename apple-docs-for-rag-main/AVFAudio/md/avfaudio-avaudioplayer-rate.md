

- AVFAudio
- AVAudioPlayer
-  rate 

Instance Property

# rate

The audio player’s playback rate.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var rate: Float { get set }
```

## Discussion

To set an audio player’s playback rate, you must first enable the rate adjustment by setting its enableRate property to true.

The default value of this property is `1.0`, which indicates that audio playback occurs at standard speed. This property supports values in the range of `0.5` for half-speed playback to `2.0` for double-speed playback.

Note

Adjusting the audio’s playback rate doesn’t alter its pitch.

## See Also

### Configuring playback settings

var volume: Float

The audio player’s volume relative to other audio output.

func setVolume(Float, fadeDuration: TimeInterval)

Changes the audio player’s volume over a duration of time.

var pan: Float

The audio player’s stereo pan position.

var enableRate: Bool

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

var numberOfLoops: Int

The number of times the audio repeats playback.

