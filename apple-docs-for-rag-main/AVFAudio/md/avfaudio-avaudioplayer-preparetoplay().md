

- AVFAudio
- AVAudioPlayer
-  prepareToPlay() 

Instance Method

# prepareToPlay()

Prepares the player for audio playback.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func prepareToPlay() -> Bool
```

## Return Value

true if the system successfully prepares the player; otherwise, false.

## Discussion

Calling this method preloads audio buffers and acquires the audio hardware necessary for playback. This method activates the audio session, so pass false to setActive:error: if immediate playback isn’t necessary. For example, when using the category option duckOthers, this method lowers the audio outside of the app.

The system calls this method when using the method play(), but calling it in advance minimizes the delay between calling `play()` and the start of sound output.

Calling stop(), or allowing a sound to finish playing, undoes this setup.

## See Also

### Controlling playback

func play() -> Bool

Plays audio asynchronously.

func play(atTime: TimeInterval) -> Bool

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

func pause()

Pauses audio playback.

func stop()

Stops playback and undoes the setup the system requires for playback.

var isPlaying: Bool

A Boolean value that indicates whether the player is currently playing audio.

