

- AVFAudio
- AVAudioPlayer
-  stop() 

Instance Method

# stop()

Stops playback and undoes the setup the system requires for playback.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func stop()
```

## Discussion

Calling this method undoes the resource allocation the system performs in prepareToPlay() or play(). It doesn’t reset the player’s currentTime value to `0`, so playback resumes from where it stops.

## See Also

### Controlling playback

func prepareToPlay() -> Bool

Prepares the player for audio playback.

func play() -> Bool

Plays audio asynchronously.

func play(atTime: TimeInterval) -> Bool

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

func pause()

Pauses audio playback.

var isPlaying: Bool

A Boolean value that indicates whether the player is currently playing audio.

