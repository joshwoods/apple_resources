

- AVFAudio
- AVAudioPlayerNode
-  stop() 

Instance Method

# stop()

Clears all of the node’s events you schedule and stops playback.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stop()
```

## Discussion

Clears all events you schedule, including any events in the middle of playing. It resets the node’s sample time to `0`, and doesn’t proceed until the node starts again through play() or play(at:).

Pausing or stopping all of the players you connect to an engine doesn’t pause or stop the engine or the underlying hardware. You must explicitly pause or stop the engine for the hardware to stop. When your app doesn’t need to play audio, pause or stop the engine to minimize power consumption.

## See Also

### Controlling Playback

func prepare(withFrameCount: AVAudioFrameCount)

Prepares the file regions or buffers you schedule for playback.

func play()

Starts or resumes playback immediately.

func play(at: AVAudioTime?)

Starts or resumes playback at a time you specify.

var isPlaying: Bool

A Boolean value that indicates whether the player is playing.

func pause()

Pauses the node’s playback.

