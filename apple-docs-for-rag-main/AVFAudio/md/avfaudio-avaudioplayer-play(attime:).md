

- AVFAudio
- AVAudioPlayer
-  play(atTime:) 

Instance Method

# play(atTime:)

Plays audio asynchronously, starting at a specified point in the audio output device’s timeline.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func play(atTime time: TimeInterval) -> Bool
```

## Parameters 

`time`  

The audio device time to begin playback. This time must be later than the device’s current time.

## Return Value

true if playback starts successfully; otherwise, false.

## Discussion

Use this method to precisely synchronize the playback of two or more audio player objects as the following example shows:

```
func startSynchronizedPlayback() {
    // Create a time offset relative to the current device time.
    let timeOffset = playerOne.deviceCurrentTime + 0.01

    // Start playback of both players at the same time.
    playerOne.play(atTime: timeOffset)
    playerTwo.play(atTime: timeOffset)
}
```

Calling this method implicitly calls prepareToPlay() if the audio player is unprepared for playback.

## See Also

### Controlling playback

func prepareToPlay() -> Bool

Prepares the player for audio playback.

func play() -> Bool

Plays audio asynchronously.

func pause()

Pauses audio playback.

func stop()

Stops playback and undoes the setup the system requires for playback.

var isPlaying: Bool

A Boolean value that indicates whether the player is currently playing audio.

