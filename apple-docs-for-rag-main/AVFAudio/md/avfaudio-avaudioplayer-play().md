

- AVFAudio
- AVAudioPlayer
-  play() 

Instance Method

# play()

Plays audio asynchronously.

iOS 2.2+iPadOS 2.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func play() -> Bool
```

## Return Value

true if playback starts successfully; otherwise, false.

## Discussion

Calling this method implicitly calls prepareToPlay() if the audio player is unprepared for playback.

## See Also

### Controlling playback

func prepareToPlay() -> Bool

Prepares the player for audio playback.

func play(atTime: TimeInterval) -> Bool

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

func pause()

Pauses audio playback.

func stop()

Stops playback and undoes the setup the system requires for playback.

var isPlaying: Bool

A Boolean value that indicates whether the player is currently playing audio.

