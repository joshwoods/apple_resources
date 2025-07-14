

- AVFAudio
- AVAudioPlayer
-  numberOfLoops 

Instance Property

# numberOfLoops

The number of times the audio repeats playback.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var numberOfLoops: Int { get set }
```

## Discussion

The default value of `0` results in the sound playing once. Set a positive integer value to specify the number of times to repeat the sound. For example, a value of `1` plays the sound twice: the original sound and one repetition. Set a negative integer value to loop the sound continuously until you call the stop() method.

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

var rate: Float

The audio player’s playback rate.

