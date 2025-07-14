

- AVFAudio
- AVAudioPlayerNode
-  play() 

Instance Method

# play()

Starts or resumes playback immediately.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func play()
```

## Discussion

This is equivalent to play(at:) with a value of `nil`.

## See Also

### Controlling Playback

func prepare(withFrameCount: AVAudioFrameCount)

Prepares the file regions or buffers you schedule for playback.

func play(at: AVAudioTime?)

Starts or resumes playback at a time you specify.

var isPlaying: Bool

A Boolean value that indicates whether the player is playing.

func pause()

Pauses the node’s playback.

func stop()

Clears all of the node’s events you schedule and stops playback.

