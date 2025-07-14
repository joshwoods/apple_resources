

- AVFAudio
- AVAudioPlayer
-  enableRate 

Instance Property

# enableRate

A Boolean value that indicates whether you can adjust the playback rate of the audio player.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var enableRate: Bool { get set }
```

## Discussion

To enable modifying the player’s rate, set this property to true after you create the player, but before you call prepareToPlay().

## See Also

### Configuring playback settings

var volume: Float

The audio player’s volume relative to other audio output.

func setVolume(Float, fadeDuration: TimeInterval)

Changes the audio player’s volume over a duration of time.

var pan: Float

The audio player’s stereo pan position.

var rate: Float

The audio player’s playback rate.

var numberOfLoops: Int

The number of times the audio repeats playback.

